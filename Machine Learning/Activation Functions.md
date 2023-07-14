Neural networks all require an activation function to properly operate. Activation functions include those such as sigmoid functions, linear functions and most commonly in neural networks, ReLU activation functions. Each activation function excels in certain areas in the neural network. A ReLU function almost always becomes the best option for the activation function of the hidden layers in a neural network. With the output layer of a neural network being more specific to the problem at hand, a ReLU function is good for determining any output where the number can go below 0, a linear activation function is good for any problem where the output is positive or negative and a sigmoid activation function is good for determining the probability of a set outcome. 

## But what exactly is an activation function?
At its core, an activation function decides whether or not a node is active or not. It decides how important the score created through the linear function wx+b is. To transform the summed weighted input from the node into an output value to be fed to the next hidden layer or as output.

## How do they work?
Activation functions are used in all [[machine learning]] problems, they are used to transform the linear graph created by the w and b parameters into something more useful for the machine. A sigmoid function is good at classifying the data into a 1 or 0 output.

### ReLU Activation
$g(z)=max(0,z)$

### Linear Activation
sometimes this is called the "no activation function"
$g(z)=z$

### Sigmoid Activation
$g(z)=\frac{1}{1+e^-z}$

### Softmax Activation
Softmax activation is a special type of activation function typically used in the output layer of a neural network to determine the likelihood a given input is a certain pre determined case. If you were classifying hand written digits, the softmax activation output would tell you the probability of each node being a pre determined case of a number between 0 and 9. To summarize the softmax activation function tells you the probability that a given input is a certain case. softmax activation functions give you the probability of all cases, so by selecting the one with the highest probability you can determine that that is the correct output.\

$$ 
a_{n}=g(z) = \frac{e_{n}^z}{\sum_{i=1}^{y}(e_{i}^z)}
$$
wherein y = total outputs and n is the case by which that function tests for. 