[[Cost or loss functions|Cost functions]] can be modified to implement "regularisation" wherein cost functions penalise functions which overfit the project [[Weights and Biases|parameters]] to [[features vs examples|examples]]. Achieved through penalising large [[Weights and Biases|w values]] which causes the final function to adopt a smoother less jittery and overfit function. Regularisation of the [[Weights and Biases|b value]] is not important![[Pasted image 20230829135210.png]]

## Implementation
$$
J(\vec{w},b) = J(\vec{w},b)+\frac{\lambda}{2m}\sum_{j=1}^nw_j^2
$$
Where $\lambda$ represents the "regularisation parameter" which is chosen based upon how important it is to reduce overfitting is. If it is too high the model will underfit the data as all parameters essentially equal 0, creating the final model where f(x) = b without the w. 