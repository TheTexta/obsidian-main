There are tons of different machine learning models used for various problems.

[[Logistic Regression]]
A simple model which gives an output between 0 and 1 of the probability of a input belonging to a label. Uses a [[Sigmoid Activation]] function for the final layer of the model to perform binary classification.

[[Linear Regression]]
A simple model which takes an input and gives it a numerical output. Basically fits a line to example variables and gives predictions based on that line. Simple [[linear regression]] involves one input [[features vs examples|feature]] while multiple [[Linear Regression|linear regressions]] involves more.

[[Multi-Class Classification]]
A model which attaches a single label of many to an input. The model uses the [[Softmax Activation]] function to produce probabilities of each label belonging to the input. All values in the vector output must add to 1. This approach uses a [[Cross entropy loss function]] to grade the model based on its category predictions. This is a neural network model, utilising multiple hidden [[Layers]] to produce an output.

[[Multi-label classification]]
A [[Neural Networks|neural network]] model which attaches one or more labels to a given input.

[[Binary Classification]]
A model which classifies an input into a yes/no result. 