#math133 

## Part 1

##### Identity Matrix
$I_n$ or just $I$ (size through context) is the $n\times n$ [[matrix]] with columns $e_1,e_2,...,e_n$ ([[standard basis vectors]])
$$I_4=\pmatrix{1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&1}$$
##### Matrix Rank
for any [[matrix]] the number of leading ones in the [[reduced row echelon form|RREF]] is the rank
##### Matrix Inverses/Invertible's
If we have matrix $A$ the inverse matrix is $A^{-1}$. We find it with the $AA^{-1}=I$ formula where we simply solve the A matrix with I as the coefficient matrix. A matrix is invertible if its RREF form is the identity matrix.
$$\pmatrix{A\vert I}=A^{-1} \text{ - solve for the LHS to get }A^{-1}$$
###### Inverse of a 2x2 matrix
Let $A=\pmatrix{a&b\\c&d}$. Define the determinant of $A$ by:
$$det(A)=ad-bc$$
If $det(A)\neq 0$ then $A$ invertible and $$A^{-1}=\frac{1}{det(A)}\pmatrix{d&-b\\-c&a}$$
###### Properties
 1. $I^{-1}=I$ - of $II=I$.
 2. If $A$ invertible $A^{-1}$ also invertible. $(A^{-1})^{-1}=A$ $$A^{-1}A=I$$
 3. *very important*. If $A$, $B$ both $n\times n$ invertible then $AB$ is invertible and $$(AB)^{-1}=B^{-1}A^{-1}$$
 4. If $A_1, A_2, ..., A_k$ all $n\times n$ invertible then $A_1,A_2,...,A_k$ is invertible and $$\pmatrix{A_1&A_2&...&A_k}^{-1}=A_k^{-1},A_k^{-1},...,A_2^{-1}$$
 5. If $A$ invertible, $m\geq 1$ (int) then $$A^m \text{ is invertible and } (A^m)^{-1}=(A^{-1})^m$$
 6. If $A$ invertible and $c\in \mathbb{R}$, $c\neq 0$ then $cA$ is invertible and $$(cA)^{-1}=\frac{1}{c}A^{-1}$$
 7. If $A$ invertible $A^T$ also invertible and $$(A^T)^{-1}=(A^{-1})^T$$
###### Prove $A$ is not invertible if $A^n = 0$
1. $A^n=0$
2. $(A^n)(A^n)^{-1}=I$
3. $0(A^n)^{-1}=I$
4. $0\neq I$
Therefor A is not invertible. 
###### Show A is invertible if $A^n=I$
$A^{−1}=A^{n−1}$ since $A^{n−1}A=A^n=I$.
##### Matrix Adjugate - I DON'T UNDERSTAND THIS
$$A^{-1}=\frac{\text{adj}(A)}{\text{det}(A)}$$
##### Elementary Matrices
$$\pmatrix{1&0&0\\3&1&0\\0&0&1}\pmatrix{a&b&c\\d&e&f\\g&h&i}=\pmatrix{a&b&c\\3a+d&3b+e&3c+f\\g&h&i}$$
##### Matrix Transposition
The transpose of a $m \times n$ [[matrix]] $A$ is the $n \times m$ matrix $A^T$ whose $(i,j)$ entry is the $(j,i)$ entry of A. 
$$A=\pmatrix{1&2&3\\4&5&6}\quad\quad A^T=\pmatrix{1&4\\2&5\\3&6}$$
###### Symmetric matrix
A [[matrix]] is $A$ is called [[symmetric matrix|symmetric]] if when [[Matrix Tranposition|transposed]] nothing changes. A symmetric matrix must be $n \times n$.
###### Properties
1. $(AB)^T=B^TA^T$
2. $(A^T)^T=A$
3. $(cA)^T=c(A^T)$
4. $(A+B)^T=A^T+B^T$
###### Properties
1. $(A^T)^T=A$
2. $(cA)^T=c(A^T)$
3. $(A+B)^T=A^T+B^T$

##### Matrix-Vector Multiplication
same as matrix matrix multiplication which is below
###### Properties
Let $A,B$ be $m\times n$ matrices, $\vec{v},\vec{w}\in\mathbb{R}^n, c\in\mathbb{R}$. Then
1. $A(\vec{v}+\vec{w})=A\vec{v}+A\vec{w}$
2. $A(c\vec{v})=c(A\vec{v})$ (LHS is $\in\mathbb{R}^n$ while RHS is $\in\mathbb{R}^m$ since the scalar expands number of solutions??)
3. $(A+B)\vec{v}=A\vec{v}+B\vec{v}$
##### Matrix-Matrix multiplication
###### Properties
1. NOT COMMUTATIVE $AE_1E_2E_3 \neq E_3E_2E_1A$ because $E_1A\neq AE_1$. 

###### Vector-Vector dot product
A special case of matrix matrix multiplication. Scalar result of multiplication of vectors of same dimension. 
If $\vec{v}=[\matrix{a_1&...&a_n}]$ and $\vec{w}=[\matrix{b_1&...&b_n}]$ -  $\vec{v}\cdot \vec{w}=\sum_{u=1}^n{a_ub_u}$. 
##### General Form Solutions
say we have these system of linear equations:
1. $x−2y−z+3w=1$
2. $2x−4y+z=5$
3. $x−2y+2z−3w=4$
which row reduces to:
$$\begin{pmatrix} 1 & -2 & -1 & 3 & \vert & 1 \\ 0 & 0 & 3 & -6 & \vert & 3 \\ 0 & 0 & 0 & 0 & \vert & 0 \end{pmatrix}$$
the ***general solution*** would henceforth be:
$$
\begin{pmatrix}
x \\
y \\
z \\
w
\end{pmatrix}
=
\begin{pmatrix}
2 + 2u - v \\
u \\
2v + 1 \\
v
\end{pmatrix}, \quad u, v \in \mathbb{R}
$$
##### Consistent vs. Inconsistent Solutions
A matrix is consistent if it has *at least one* solution. It is inconsistent otherwise. 

##### Free Variables
- \# of variables matrix rank free variables
##### Homogeneous system
All constants are zero.
## Part 2
##### Determinants
###### 3x3
$$\det{\pmatrix{4&-1&1\\4&5&3\\-2&0&0}}=(+)(4)\cdot \det{\pmatrix{5&3\\0&0}} + (-)(-1)\det\pmatrix{4&3\\-2&0}+(+)(1)\det\pmatrix{4&5\\-2&0}=16$$
###### 4x4+
You can add rows to others without changing the determinant. Use this to get to upper triangular form and compute the determinants by taking the product of the diagonal entries. Otherwise can use same method as above but will take fucking forever.
$$\det\pmatrix{1&2&2&1\\1&2&4&2\\2&7&5&2\\-1&4&-6&3}=\det\pmatrix{1&2&2&1\\0&3&3&1\\0&0&-2&-1\\0&0&0&7}=1\cdot3\cdot-2\cdot7=-42$$
###### Splitting Determinants
Let $A,B$ $n\times n$ then,
$det(AB)=det(A)\cdot det(B)$
###### Inverse determinant relationship
$$det (A^{-1})=\frac{1}{det(A)}$$
###### Inverse and power relationship
$$$det(A^m)=det(A)^m$$
##### Inverses
$$(A:I)->(I:A^{-1})$$

##### Markov Chains
A population migration model. Regions ABC exist. Each year:
- From A, 10% moves to B, 20% to C, 70% stay
- From B, 5% to A, 20% to C, 75% stay
- from C, 5% to A, 5% to B, 90% stay
Forms the transition matrix:
$$\pmatrix{0.7&0.05&0.05\\0.1&0.75&0.05\\0.2&0.2&0.9}=T$$
Where in general, if $\vec{P}_n=$pop in year $n$, if multiply $T\vec{p}_n=\vec{P}_{n+1}$. Also if $T$ inv, $T^{-1}$ will do backwards year prop. Where P is of form $\pmatrix{A\\B\\C}$.
##### Invertible's
A matrix which has an inverse matrix whose product results in the identity matrix is "invertible." $$\text{A matrix is invertible} \iff det(A)\neq0$$
##### Cofactor Matrix
$$A=\begin{pmatrix} -1 & -2 & 2 \\ 2 & 1 & 1 \\ 3 & 4 & 5 \end{pmatrix} \text{cofactor of A is }$$$$ C= \text{matrix of minors} \rightarrow \begin{pmatrix} \begin{vmatrix} 1 & 1 \\ 4 & 5 \end{vmatrix} & \begin{vmatrix} 2 & 1 \\ 3 & 5 \end{vmatrix} & \begin{vmatrix} 2 & 1 \\ 3 & 4 \end{vmatrix} \\ \begin{vmatrix} -2 & 2 \\ 4 & 5 \end{vmatrix} & \begin{vmatrix} -1 & 2 \\ 3 & 5 \end{vmatrix} & \begin{vmatrix} -1 & -2 \\ 3 & 4 \end{vmatrix} \\ \begin{vmatrix} -2 & 2 \\ 1 & 1 \end{vmatrix} & \begin{vmatrix} -1 & 2 \\ 2 & 1 \end{vmatrix} & \begin{vmatrix} -1 & -2 \\ 2 & 1 \end{vmatrix} \end{pmatrix} = \begin{pmatrix} 1 & 7 & 5 \\ -18 & -11 & 2 \\ -4 & -5 & 3 \end{pmatrix}$$
$$\quad \text{checkerboard pattern} \rightarrow \pmatrix{1&-7&5\\18&-11&-2\\-4&5&3}$$
##### Adjoint Matrix
$$C^T=adj(C)$$
Property 1:
$$A\cdot adj(C)=\pmatrix{det(A)&0&0\\0&det(A)&0\\0&0&det(A)}$$
Property 2:
$$A^{-1}=\frac{1}{det(A)}\cdot adj(A)$$
##### Polynomial Interpolation
With $n+1$ points can find polynomial $f(x)$ such that $f(x_i)=y_i$ for all $i$. this can be done with polynomial of degree $n$ where $n=i-1$. 
$$\begin{pmatrix} 1 & x_0 & x_0^2 & \dots & x_0^n \\ 1 & x_1 & x_1^2 & \dots & x_1^n \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 1 & x_n & x_n^2 & \dots & x_n^n \\ \end{pmatrix} \begin{pmatrix} a_0 \\ a_1 \\ a_2 \\ \vdots \\ a_n \\ \end{pmatrix} = \begin{pmatrix} y_0 \\ y_1 \\ \vdots \\ y_n \\ \end{pmatrix}$$
e.g.
You are given the points $(x_0,y_0)=(1,2)$, $(x_1,y_1)=(2,3)$, and $(x_2, y_2) = (3, 5)$. Find the polynomial $f(x)$ of degree $n=3-1=2$ that passes through these points.
$$\pmatrix{1&1&1^2\\1&2&2^2\\1&3&3^2}\pmatrix{a_0\\a_1\\a_2}=\pmatrix{2\\3\\5}$$
forms augmented matrix which reduces to the right.
$$\pmatrix{1&1&1&2\\1&2&4&3\\1&3&9&5}\rightarrow\pmatrix{1&0&0&2\\0&1&0&-\frac{1}{2}\\0&0&1&\frac{1}{2}}$$
therefor
$$a_0=2, a_1=-\frac{1}{2},a_2=\frac{1}{2}$$
forming the polynomial
$$f(x)=2-\frac{1}{2}x+\frac{1}{2}x^2$$
