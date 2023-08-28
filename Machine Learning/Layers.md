[[Neural networks]] all have at least a an input layer, 1 hidden layer and a output layer. These layers operate on [[arrays]] of data denoted by the [[Alpha value|alpha]] $\vec{a}$ symbol. All layers transform each input they are given to create new values which suit the purpose of that individual [[Nodes]] within the layer which is transforming it. In the t-shirt problem you would have at least one [[Nodes]] for predicting the perceived value of the shirt.

## Hidden layers
Hidden layers are the layers which actually do all the work in the [[machine learning]] process despite there misleading name. Hidden layers take all the inputs and extract important features that more closely correlate with the variables which one needs to find the desired output of the neural network. In the t-shirt example, the hidden layer takes data on the price and perceived quality of a t-shirt and gives it a desirability score which by itself would be impossible to measure.

## How to read layer script
$$
W_{j}^{n} = \text{jth weight of the nth layer}
$$


# Types of Layers
## Dense layers
Dense layers are a function of all previous layers in a function. They take the last layers output and transform it in some way to be passed onto the next layer. Dense layers consist of many neurons which each take the whole output of the previous layer and transform that data in a unique way. 

## Convolutional Layer
Each neuron in a convolutional layer only looks at part of the previous layers outputs. As opposed to a dense layer which always looks at the whole output of the previous layer and transforms all of those input in some way. Convolution layers have numerous benefits, decreased risk to overfitting, faster computations, less training data necessary, etc. In a way convolution layers look at a "window" of the data input. 