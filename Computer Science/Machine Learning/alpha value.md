Within machine learning the alpha value controls how "fast" a machine learning algorithm optimises its [[Cost or loss functions]] to fit a given dataset. It controls how much the [[Weights and Biases]] are updated by by controlling the impact of the [[Derivative]] of the [[Cost or loss functions]] through a multiplication of the cost function by the [[Derivative]] of the [[Cost or loss functions]]

For a given parameter w:
$$w= w - \alpha\cdot\frac{d}{dx}(J(x))$$

If a the alpha value is too large then the algorithm can take too long to find its local minima as it overshoots. If it is too small then the algorithm will take a long time to compute. 
![[over-under shoot of gradient descent.png]]