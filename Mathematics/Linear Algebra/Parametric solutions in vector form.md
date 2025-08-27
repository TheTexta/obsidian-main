#math133 
#### Ex 
[[Augmented matrix]] variables $x_1,x_2,x_3,x_4$
$\pmatrix{1&2&0&-4&|1\\0&0&1&3&|2}$

$x_2$ and $x_4$ are [[free variables]]. 

*Solution* (parametric form)
$x_1=1-2s+4t$
$x_2=s$
$x_3=2-3t$
$x_4=t$

*Solution* (vector form) (we can solve these through [[Linear combination of matrices|linear combination]])
$\vec{X}=\pmatrix{x_1\\x_2\\x_3\\x_4}=\pmatrix{1-2s+4t\\0+s+0t\\2+0s-3t\\0+0s+t}$ 
$=\pmatrix{1\\0\\2\\0}+\pmatrix{-2s\\s\\0\\0}+\pmatrix{4t\\0\\-3t\\t}$
$=\pmatrix{1\\0\\2\\0}+s\cdot\pmatrix{-2\\s\\0\\0}+t\cdot\pmatrix{4\\0\\-3\\t}$
$=\text{some vector}+\text{any lin comb of two other specific vectors}$


