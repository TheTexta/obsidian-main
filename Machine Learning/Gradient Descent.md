Gradient descent is a method for algorithm optimization which uses the [[derivative]] of the cost formula to find the optimal changes which can be incrementally implemented into the [[Weights and Biases]] of the algorithm.![[gradient descent ex.png]]
## How does gradient descent work for algorithms?
Gradient descent is used to optimize the entire algorithm, not just the single [[Weights and Biases|weight/biases]] which is being updated. Its important to note that when there are multiple [[features vs examples]] in a problem, the weights are each updated with an independent value but all the independent values point towards a local minima that will optimize ALL values of a function not just the value which is being updated. This is why it is important that the cost function takes into account all previous [[Weights and Biases|weights]] when updating a single weight parameter.

# What is the algorithm mathematically?
$$ 
W_j=W_j-\alpha\frac{\partial}{\partial W_j}J(\vec{w}, b)
$$
Here, we take the initial weight param and adjust it by the derivative of the cost function in an attempt to reach the local minima of the cost function. The $\alpha$ represents the learning rate of the function. By adjusting this learning rate one can improve the effeciency of the algorithm but at the cost of increased risk in overshoot.