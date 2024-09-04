Computers aren't very good at storing fractions. depending on how you calculate with them the computer can be prone to roundoff errors, wherein fractional computations gradually decrease in numerical accuracy as increasing numbers of operations are performed on them as they are only able to store so many digits. 

## Examples of numerical roundoff error
Say you want to compute the value of $\frac{2}{10000}$, if you were to do
```python
x1 = 2.0/10000
print(f"{x1:.18f}")
--------------------------------------------------------------------------------------
0.0002000000000000000000
```
but if you instead computed the value of $\frac{1}{10000}$ with the formula $1+(\frac{1}{10000}) - (1-\frac{1}{10000})$
you would run into numerical roundoff errors.
```python
x2 = 1+(1/10000)-(1-1/10000)
print(f"{x1:.18f}")
--------------------------------------------------------------------------------------
0.0001999999999999999978
```

## Disadvantages of the use_logits method
When using the use_logits in the compilation of models its  important to remember to set the output layer to use a linear activation function for the optimisation to work. You then have to apply SoftMax to the logit output of the model in order to get the normalised probability of each classification in a classification problem (multiclass or binary). 

Normally when a model is used for a binary classification problem, the given output of the function is squashed in the last layer into a number between 0 and 1 to give the probability that it belongs to the two categories. Achieved through the sigmoid function $f(z) = \frac{1}{1+e^-z}$ where z is the logit output of the previous to last layer. When logits are specified and a linear output is requested, the final output of the function will be the unnormalized result, so we have to apply the sigmoid function manually. 

Similar applies for the multiclass classification where the softmax function is used in place of the sigmoid one. 
