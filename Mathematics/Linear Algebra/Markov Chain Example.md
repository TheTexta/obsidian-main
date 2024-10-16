#math133 
A population migration model. Regions ABC exist. Each year:
- From A, 10% moves to B, 20% to C, 70% stay
- From B, 5% to A, 20% to C, 75% stay
- from C, 5% to A, 5% to B, 90% stay

Define transition matrix:
A - b - c from
$\pmatrix{0.7&0.05&0.05\\0.1&0.75&0.05\\0.2&0.2&0.9}=T$

if population in 2020 is $\vec{P}_0=\pmatrix{300\\200\\100}$ then multiply matrix be vector for next year.
$T\vec{P}_0=\pmatrix{0.7&0.05&0.05\\0.1&0.75&0.05\\0.2&0.2&0.9}\pmatrix{300\\200\\100}$=population in next year 2021. 

In general, if $\vec{P}_n=$pop in year $n$, if multiply $T\vec{p}_n=\vec{P}_{n+1}$. Also if $T$ inv, $T^{-1}$ will do backwards year prop.

Q. How to compute $T^n$ efficiently?
Q. What happens in long term? In long term pop. stabilises to $\vec{p}$=87.5, 114.3 and 400. In fact $T\vec{p}=\vec{p}$. p is called a steady stable vector. 