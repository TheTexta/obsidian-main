#math133 
You actually *cannot* multiply a vectors by another but you can take the [[dot product]]. 

Let $A=[\matrix{\vec{v_1}&\vec{v_2}&...&\vec{v_n}}]$ be $m\times n$ [[matrix]] each $v_i \in \mathbb{R}^m$ (ie $m \times 1$ [[column vector]]) and let $\vec{x}=\pmatrix{x_1\\x_2\\...\\x_n}\in\mathbb{R}$. we define the product $A\vec{x}$ as the [[vector]] in $\mathbb{R}^m, a\vec{x}=x_1v_1 + x_2v_2 + ... + x_nv_n$ ie combine columns of A according to number $m\vec{x}$. 

##### Example
$A=\pmatrix{1&2&3\\4&5&6} \quad \vec{x}=\pmatrix{3\\-1\\2}$
then
$A\vec{x}=3\pmatrix{1\\4} -(1)\pmatrix{2\\5} + 2 \pmatrix{3\\6}$ 

$\quad \quad = \pmatrix{3&-2&6\\12&-5&12}=\pmatrix{7\\19}$   

##### Properties of Matrix-Vector Multiplication
Let $A,B$ be $m\times n$ matrices, $\vec{v},\vec{w}\in\mathbb{R}^n, c\in\mathbb{R}$. Then
1. $A(\vec{v}+\vec{w})=A\vec{v}+A\vec{w}$
2. $A(c\vec{v})=c(A\vec{v})$ (lhs is $\in\mathbb{R}^n$ while rhs is $\in\mathbb{R}^m$ since the scalar expands number of solutions??)
3. $(A+B)\vec{v}=A\vec{v}+B\vec{v}$

*1 and 2 known as linearity properties*

##### Proof of Properties
1. 
$$
\text{Let } A=\pmatrix{\vec{u}_1,\vec{u}_2,...,\vec{u}_n},\vec{v}=\pmatrix{a_1\\...\\a_n}, \vec{w}=\pmatrix{b_1\\...\\b_n}
$$
Then
$$
\matrix{
A(\vec{v}+\vec{w})&=&A\pmatrix{a_1+b_1\\a_2+b_2\\...\\a_n+b_n}\\

&=&(a_1+b_1)\vec{u}_1+(a_2+b_2)\vec{u}_2+...+(a_n+b_n)\vec{u}_n\\

&=&a_1\vec{u}_1+b_1\vec{u}_1+...+a_n\vec{u}_n+b_n\vec{u}_n\\

&=&(a_1\vec{u}_1+...+a_n\vec{u}_n) + (b_1\vec{u}_1+...+b_n\vec{u}_n)\\

&=&A\vec{v}+A\vec{w}
}
$$
2. (self proof)
$$
\text{Let } A=\pmatrix{\vec{u}_1,\vec{u}_2,...,\vec{u}_n},\vec{v}=\pmatrix{a_1\\...\\a_n},c\in\mathbb{R}
$$
Then
$$
\matrix{
A(c\vec{v})&=&A\pmatrix{ca_1\\ca_2\\...\\ca_n}\\

&=&\pmatrix{\vec{u}_1&\vec{u}_2&...&\vec{u}_n}\pmatrix{ca_1\\ca_2\\...\\ca_n}\\
&=&\sum\limits_{i=1}^n ca_i \vec{u_i}\\
&=&c\sum\limits_{i=1}^n a_i \vec{u_i}\\
&=&c\cdot(\vec{v}A)
}
$$
3. (self proof)
$$
\text{Let } A=\pmatrix{\vec{u}_1,\vec{u}_2,...,\vec{u}_n},B=\pmatrix{\vec{x}_1,\vec{x}_2,...,\vec{x}_n},\vec{v}=\pmatrix{a_1\\...\\a_n}
$$
$$
\matrix{
(A+B)\vec{v}&=&(\pmatrix{\vec{u}_1,\vec{u}_2,...,\vec{u}_n}+\pmatrix{\vec{x}_1,\vec{x}_2,...,\vec{x}_n})\pmatrix{a_1\\...\\a_n}\\

&=&\pmatrix{(\vec{u}_1+\vec{x}_1),(\vec{u}_2+\vec{x}_2),...,(\vec{u}_n+\vec{x}_n)}\pmatrix{a_1\\...\\a_n}\\

&=&\pmatrix{a_1(\vec{u}_1+\vec{x}_1),a_2(\vec{u}_2+\vec{x}_2),...,a_n(\vec{u}_n+\vec{x}_n)}\\

&=&\pmatrix{a_1\vec{u}_1+a_1\vec{x}_1,a_2\vec{u}_2+a_2\vec{x}_2,...,a_n\vec{u}_n+a_n\vec{x}_n}\\

&=&\pmatrix{a_1\vec{u}_1,a_2\vec{u}_2,...,a_n\vec{u}_n}+\pmatrix{a_1\vec{x}_1,a_2\vec{x}_2,...,a_n\vec{x}_n}\\

&=&A\vec{v}+B\vec{v}
}
$$

##### Example using properties
If $A,B m\times n$ matrices $\vec{u},\vec{v}\in\mathbb{R}^n$
then $(A+B)(2\vec{u}-3\vec{v})$ 
$=A(2\vec{u}-3\vec{v})+B(2\vec{u}-3\vec{v})$ - *Rule 3*
$= A(2\vec{u})-A(3\vec{v})+B(2\vec{u})-B(3\vec{v})$ - *Rule 1*
$= 2A(\vec{u})-3A(\vec{v})+2B(\vec{u})-3B(\vec{v})$ - *Rule 2*

