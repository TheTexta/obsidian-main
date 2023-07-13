Within machine learning the alpha value controls how "fast" a machine learning algorithm optimises its [[cost function]] to fit a given dataset. It controls how much the [[weights and biases]] are updated by by controlling the impact of the [[Derivative]] of the [[cost function]] through a multiplication of the cost function by the [[derivative]] of the [[cost function]]

For a given parameter w:
$$w= w - \alpha\cdot\frac{d}{dx}(J(x))$$

If a the alpha value is too large then the algorithm can take too long to find its local minima as it overshoots. If it is too small then the algorithm will take a long time to compute. 
![[over-under shoot of gradient descent.png]]