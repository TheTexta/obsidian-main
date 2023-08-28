Optimises the $\alpha$ learning rate of the [[gradient descent]] algorithm to adjust as the function reaches its minima. Adam stands for "adaptive moment estimation", unlike traditional gradient descent Adam uses a different learning rate $\alpha$ for each parameter in the model. 

# Implementation
The Adam algorithm can be implemented in TensorFlow when compiling the network by specification. The learning_rate just specifies the initial learning rate. By setting it to 10^-3 overshot is unlikely to occur. You can experiment with others for better efficiency.
```python
model.compile(optimizer = tf.keras.optimizers.Adam(learning_rate=le-3), loss = tf.keras.losses.SparseCategoricalCrossentropy(from_logits=true))
```
