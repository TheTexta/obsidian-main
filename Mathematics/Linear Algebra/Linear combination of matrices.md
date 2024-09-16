#math133 
Let $A_1, A_2, ... A_n$ be $m\times n$ [[Matrix|matrices]] and $c_1,c_2,...,c_n \in \mathbb{R}$. then the $m \times n$ [[matrix]] 
$$
c_1A_1+c_2A_2 + ... + c_nA_n
$$ is called a linear combination of $A_1, ..., A_n$ matrixes

#### Example

Every $2\times 2$ matrix $A=\pmatrix{a&b\\c&d}$ can be written as a linear combination of
$$
E_1=\pmatrix{1&0\\0&0}+E_2=\pmatrix{0&1\\0&0}+E_3=\pmatrix{0&0\\1&0}+E_4=\pmatrix{0&0\\0&1}
$$
 since $aE_1 + bE_2 + cE_3 + dE_4$
 $$
=\pmatrix{a&0\\0&0}+\pmatrix{0&b\\0&0}+\pmatrix{0&0\\ c&0}+\pmatrix{0&0\\0&d}=A
$$

###### Problem
Show every $\vec{v} =\pmatrix{a\\b\\c}$ can be written uniquely as linear combination of $\vec{u_1}=\pmatrix{1\\-1\\0}, \vec{u_2}=\pmatrix{0\\1\\-1}, \vec{u_3}=\pmatrix{1\\0\\1}$.
*solution*
for all $a,b,c$ can we find $x_1,x_2,x_3$ such that $x_1\vec{u_1} + x_2\vec{u_2} + x_3\vec{u_3} = \vec{v}$?
ie.
$$
x_1\pmatrix{1\\-1\\0}+x_2\pmatrix{0\\1\\-1}+x_3\pmatrix{1\\0\\1}=\pmatrix{a\\b\\c}
$$
$$
\pmatrix{x_1\\-x_1\\0}+\pmatrix{0\\x_2\\-x_2}+\pmatrix{x_3\\0\\x_3}=\pmatrix{a\\b\\c}
$$
$$
\pmatrix{x_1+x_3\\-x_1+x_2\\-x_2+x_3}=\pmatrix{a\\b\\c}
$$
ie.
$x_1+\quad+x_3=a$
$-x_1 + x_2 + \quad = b$
$\quad \quad -x_2+x_3=c$
**Solve**

$\pmatrix{1&0&1&|a\\-1&1&0&|b\\0&-1&1&|c}$ we can see after some row reduction to the form $\pmatrix{1&0&1&|&a\\0&1&1&|&a+b\\0&0&2&|&a+b+c}$  that there are 3 leading variables no free variables and it is consistent (regardless of abc) since always solution. Fore the actual linear combination (we already answered the question now) we find through [[Elementary Row Operations]] that we get this matrix:

$\pmatrix{1&0&0&|\frac{1}{2}(a-b-c)\\0&1&0&|\frac{1}{2}(a+b-c)\\0&0&1&|\frac{1}{2}(a+b+c)}$

So $\pmatrix{a\\b\\c}=\frac{1}{2}(a-b-c)\cdot \pmatrix{1\\-1\\0}+\frac{1}{2}(a+b-c)\cdot \pmatrix{0\\1\\-1}+\frac{1}{2}(a+b+c)\cdot \pmatrix{1\\0\\1}$
