The goal of logistic regression is to find [[Weights and Biases]] which fit into the algorithm
$$ f(x)=\frac{1}{1+e^(\vec{w}\vec{x}+b)} $$
Optimal values for logistic regression are obtained through reduction of the [[Cost or loss functions]] to its given minimum through [[Gradient Descent]]. The [[Cost or loss functions]] for logistic regression is defined as 
$$ J(f(x)) = -\frac{1}{m}\sum_{i=1}^{m}((y^ilog(f(x^i)))+(1-y^i)(log(1-f(x^i))) $$
$$\displaylines{ m=\text{number of training examples}
\\J = \text{Cost value with given parameters for a given feature in the training set}
\\i = \text{example from dataset}
\\j = \text{feature of training set} }$$

Updating each parameter w and b for the algorithm with the [[Derivative]] of the [[Cost or loss functions]] multiplied by the [[Alpha value]] allows for the parameters to gradually find there local minimum within a given problem. 

The [[derivative]] of the [[Cost or loss functions]] for logistic regression of the b value is:
$$\frac{dJ(w,b)}{d(b)} = \frac{1}{m}\sum_{i=1}^{m}f(x^i)-y^i$$
The [[derivative]] of the [[Cost or loss functions]] for logistic regression of the w parameters is:
$$\frac{dJ(w,b)}{d(w)} = \frac{1}{m}\sum_{i=1}^{m}(f(x^i)-y^i)x_{j}^i$$