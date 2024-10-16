Nodes are used to build layers in a [[Neural Networks|neural network]]. Each hidden [[Layers|layer]] is comprised of nodes which transform the input data into something more useful for the purpose of the nodes. 

A node takes an input, multiplies the inputs by there [[Weights and Biases|weights, adds bias]] to it all, then feeds it into the nodes chosen [[Activation Functions|activation function]], which decides how important the result is by seeing what threshold values the node begins around. 

### how do we find a loop in a node list
- two pointers one running faster than the other (p1 - one step - p2 two steps). they will meet. compute from there.
- change node class to have a boolean for each node
- slow method: outer loop with inner loop checking if it matches the outer loop element