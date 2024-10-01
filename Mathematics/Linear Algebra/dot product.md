#math133 
Let $\vec{v}=\pmatrix{a_1\\...\\a_n}\in \mathbb{R}^n$, $\vec{w}=\pmatrix{b_1\\...\\b_n}\in\mathbb{R}^n$
their dot product is the [[scalar]]
$$
\vec{v}\cdot\vec{w}=a_1b_1+...+a_nb_n=\sum^{n}_{i=1}{a_ib_i}
$$
##### dot product of two matrices
![[matrix product of two matrices.png]]
##### Observation
If $A=\pmatrix{a_1&a_2&...&a_n}$ (an $l\times n$ [[matrix]])and $\vec{w}=\pmatrix{b_1\\..\\b_n}\in\mathbb{R}^n$ ([[column vector]]) then $A\vec{w}=b_1a_1+b_2a_2+...+b_na_n$ 
So rewriting $A$ as a [[vector]] if $\vec{v}=\pmatrix{a_1\\a_2\\...\\a_n}$ then $\vec{v}\cdot\vec{w}=\vec{v}^T\vec{w}$
##### matrix-vector multiplication in dot product form
$$
\matrix{\text{let }A=[a_{ij}],\vec{v}=\pmatrix{x_1\\...\\x_n}

\\

A\vec{v}=x_1\pmatrix{a_{11}\\a_{21}\\...\\a_{m1}}+...+x_n\pmatrix{a_1n\\a_2n\\...\\a_mn}
=\pmatrix{x_1a_{11}+x_2a_{12}+...+x_na_{1n}\\\vdotswithin{}\\x_1m_{m1}+x_2a_{m2}+...+x_na_{mn}}
=\pmatrix{\vec{v}\cdot\text{row 1 of }A\\\vec{v}\cdot\text{row 2 of }A

\\ \vdotswithin{}\\\vec{v}\cdot\text{row }m\text{ of }A}}
$$



So if $A=\pmatrix{\vec{w}_1\\...\\\vec{w}_m}, \vec{w}_i=\text{row }i\text{ of }A$ then $A\vec{v}=\pmatrix{\vec{w}_1\cdot\vec{v}\\\vec{w}_1\cdot\vec{v}\\...\\\vec{w}_m\cdot\vec{v}}$

##### Example
$A=\pmatrix{2&0&4\\1&-1&2\\3&1&0}\pmatrix{1\\2\\3}=\pmatrix{2+0+12\\1-2+6\\3+2+0}=\pmatrix{14\\5\\5}$ 

### Dot Product Rule
The $(i,j)$ - entry of $AB$ is

$(AB)_{ij}=(row i of A)\cdot (column j of B)$
