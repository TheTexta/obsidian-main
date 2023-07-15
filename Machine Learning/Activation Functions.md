Neural networks all require an activation function to properly operate. Activation functions include those such as sigmoid functions, linear functions and most commonly in neural networks, ReLU activation functions. Each activation function excels in certain areas in the neural network. A ReLU function almost always becomes the best option for the activation function of the hidden layers in a neural network. With the output layer of a neural network being more specific to the problem at hand, a ReLU function is good for determining any output where the number can go below 0, a linear activation function is good for any problem where the output is positive or negative and a sigmoid activation function is good for determining the probability of a set outcome. 

## But what exactly is an activation function?
At its core, an activation function decides whether or not a node is active or not. It decides how important the score created through the linear function wx+b is. To transform the summed weighted input from the node into an output value to be fed to the next hidden layer or as output.

## How do they work?
Activation functions are used in all [[machine learning]] problems, they are used to transform the linear graph created by the w and b parameters into something more useful for the machine. A sigmoid function is good at classifying the data into a 1 or 0 output. The main activation functions are:
* [[ReLU Activation]]
* [[Linear Activation]]
* [[Sigmoid Activation]]
* [[Softmax Activation]]

