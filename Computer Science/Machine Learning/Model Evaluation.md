By splitting the input [[features vs examples|example]] data into 3 subsets the model can be further optimised for new data while also automatically selecting the best degree for the polynomial function used. The model is first optimised with the training data on 10 different polynomial degree functions. The cross validation data set is then used to select the best degree polynomial for the model. Finally, the test set is used to evaluate the models performance on unseen data. 

$m_{train} = \text{no. of training examples}$  

Using this training set we can evaluate model performance with the test error algorithm


# Linear Regression Error Tests
## Training Set
$\approx$ 60% of data in the training set is dedicated to training the different models to fit the data. 
$$
J_{test} (\vec{w},b) = \frac{1}{2m_{test}}(\sum_{i=1}^{m_{test}}(f_{\vec{w},b}(\vec{x}^i_{test})-y_{test}^{(i)})^2)
$$

$$
J_{train} (\vec{w},b) = \frac{1}{2m_{train}}(\sum_{i=1}^{m_{train}}(f_{\vec{w},b}(\vec{x}^i_{train})-y_{train}^{(i)})^2)
$$

## Cross Validation (Development Set)
This is a small portion of data which is used to evaluate the performance of different orders of polynomial models which can be selected for the algorithm. 20% of example data is used here to evaluate the resulting model of the training set algo optimise the algorithm for the best polynomial degree for the function required. The cross validation set can also be used for choosing the correct neural network architecture. You can use it to decide the number of [[Layers|hidden layers]] and the [[Nodes|units]] within those layers.

## Test Set
The same as the training error but tests the algorithm with new unseen data. Good for [[Overfitting]] identification. ****

# Classification Error Tests
![[Pasted image 20230829212229.png]]
When evaluating classification models it is more common to compare the fraction of the test set and the fraction of the training set which the algorithm has misclassified. Achieved by counting the number of $\hat{y} \neq y$ where $\hat{y}$ is the algorithms prediction.