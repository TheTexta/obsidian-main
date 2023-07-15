TensorFlow is a popular python library for developing machine learning models

### Machine learning TensorFlow implementation
Always import [[TensorFlow]]
```python
import tensorflow as tf
from tensorflow.keras import Sequential
from tensorflow.keras.layers import Dense
```
#### Logistic Regression
```python
model = Sequential ([Dense(units=25,activation='relu'),
					Dense(units=15,activation='relu'),
					Dense(units=1,activation='sigmoid')
					])
model.compile(loss=BinaryCrossEntropy)
```
The code above implements a 3 layer neural network which takes 25 inputs and outputs a single number between 0 and 1. This implementation uses the loss function of binary cross entropy which is just a fancy [[Cost or loss functions|loss function]]. The ``from_logits`` part of the code allows for [[TensorFlow]] to have greater flexibility in how it manipulates the input data and prevents [[Numerical Roundoff Error|numerical roundoff errors]]. For greater numerical accuracy the logits code is included below. The reason this code is more accurate is that it computes the z value rather then the g(z) for the model which is better for training as g(z) can often produce very small/large floating point numbers.
```python
model = Sequential ([Dense(units=25,activation='relu'),
					Dense(units=15,activation='relu'),
					Dense(units=1,activation='linear')
					])
from tensorflow.keras.losses import BinaryCrossentropy
model.compile(loss=BinaryCrossEntropy(from_logits=true))
model.fit(X,Y,epochs=100)
logit = model(X)
f_x = tf.nn.sigmoid(logit)
```
#### Softmax Output
```python
model = Sequential ([Dense(units=25,activation='relu'),
					Dense(units=15,activation='relu'),
					Dense(units=10,activation='softmax')
					])
model.compile(loss=SparseCategoricalCrossEntropy(from_logits=False))
```
for greater numerical accuracy
```python
model = Sequential ([Dense(units=25,activation='relu'),
					Dense(units=15,activation='relu'),
					Dense(units=10,activation='linear')
					])
#Compile
from tensorflow.keras.losses import SparseCategoricalCrossentropy
model.compile(loss=SparseCategoricalCrossEntropy(from_logits=True))
#Fit
model.fit(X,Y,epochs=100)
#Predict
logits = model(X)
f_x = tf.nn.softmax(logits)
```