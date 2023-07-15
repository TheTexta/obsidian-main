[[Neural networks]] all have at least a an input layer, 1 hidden layer and a output layer. These layers operate on [[arrays]] of data denoted by the $\vec{a}$ symbol. All layers transform each input they are given to create new values which suit the purpose of that individual [[Nodes]] within the layer which is transforming it. In the tshirt problem you would have at least one [[Nodes]] for predicting the perceived value of the shirt.

## Hidden layers
Hidden layers are the layers which actually do all the work in the [[machine learning]] process despite there misleading name. Hidden layers take all the inputs and extract important features that more closely correlate with the variables which one needs to find the desired output of the neural network. In the t-shirt example, the hidden layer takes data on the price and perceived quality of a t-shirt and gives it a desirability score which by itself would be impossible to measure.

## How to read layer script
$$
W_{j}^{n} = \text{jth weight of the nth layer}
$$


