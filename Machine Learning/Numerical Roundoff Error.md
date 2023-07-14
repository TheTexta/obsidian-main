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

