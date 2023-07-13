The goal of logistic regression is to find [[weights and biases]] which fit into the algorithm
$$ f(x)=\frac{1}{1+e^(\vec{w}\vec{x}+b)} $$
Optimal values for logistic regression are obtained through reduction of the [[cost function]] to its given minimum through [[Gradient Descent]]. The [[cost function]] for logistic regression is defined as 
$$ J(f(x)) = -\frac{1}{m}\sum_{i=1}^{m}((y^ilog(f(x^i)))+(1-y^i)(log(1-f(x^i))) $$
$$\displaylines{ m=\text{number of training examples}
\\J = \text{Cost value with given parameters for a given feature in the training set}
\\i = \text{example from dataset}
\\ }$$

Updating each parameter w and b for the algorithm with the [[Derivative]] of the [[cost function]] multiplied by the [[alpha value]] allows for the parameters to gradually find there local minimum within a given problem. 