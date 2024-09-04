Softmax activation is a special type of [[Activation Functions|activation function]] typically used in the output [[Layers|layer]] of a [[Neural Networks|neural network]] to determine the likelihood a given input is a certain pre determined case. If you were classifying hand written digits, the softmax activation output would tell you the probability of each [[Nodes|node]] being a pre determined case of a number between 0 and 9. To summarize the softmax activation function tells you the probability that a given input is a certain case. softmax [[Activation Functions]] give you the probability of all cases, so by selecting the one with the highest probability you can determine that that is the correct output.

$$ 
a_{n}=g(z) = \frac{e_{n}^z}{\sum_{i=1}^{y}(e_{i}^z)}
$$
wherein y = total outputs and n is the case by which that function tests for. 