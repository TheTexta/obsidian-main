#math133 
A $m\times n$ matrix of form where $\lambda_i$ is any value is called a diagonal matrix.
$$\mathbf{D} = 
\begin{pmatrix}
\lambda_1 & 0 & \cdots & 0 \\
0 & \lambda_2 & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & \lambda_n
\end{pmatrix}
$$

Two important roles
1.
$$\mathbf{D}^m = 
\begin{pmatrix}
\lambda_1^m & 0 & \cdots & 0 \\
0 & \lambda_2^m & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & \lambda_n^m
\end{pmatrix}, m\geq 1$$

2.
$De_i=\lambda_i e_i$
As a linear transformation, $D$ can be described as rescaling along each coordinate axis.
ex.
$$D=\pmatrix{2&0\\0&3}$$

A $n\times n$ matrix if $v$ is a nonzero vector in $R^n$ and
$$Av=\lambda v$$
then $v$ called an eigenvector of $A$ with eigenvalue $\lambda$.
Similarly if $T:R^n->R^n$ and $T(v)=\lambda v$ for $v\neq \vec{0}$ then $v$ eigenvector for eigenvalue $\lambda$.
Ex
$$\pmatrix{2&0&0\\1&2&-1\\1&3&-2}\pmatrix{1\\1\\1}=\pmatrix{2\\2\\2}=2\pmatrix{1\\1\\1}$$ so $\pmatrix{1\\1\\1}$ is an eigenvector for $\lambda =2$. Since the vector gets scaled by a factor of $2$ for all values exactly - the vector doesn't change the direction its pointed with its just scaled by the matrix without anything else changing. other vectors would have additional transformations applied other than being simply scaled. the eigenvalue ($\lambda$) here is $2$. 

Ex. $T:R^3-R^3$ be the rotation about the z-axis by $\pi$. So all $\pmatrix{0\\0\\z}$ are eigenvectors for $\lambda =1$. $T\pmatrix{x\\y\\0}=-\pmatrix{x\\y\\0}$ eigenvectors $\lambda =-1$. 

1. $\vec{0}$ does not count as eigenvector (since then every $\lambda$ would be eigenvalue).
2. If $Av=\vec{0}$ for some $v\neq 0$ so $\lambda=0$ would be eigenvalue. 

$\lambda=0$ is eigenvalue $\iff$ Av=0v=0 for some $v\neq v$. 
$\lambda=0$ is eigenvalue $\iff$ Sys. Ax=0 has nontrivial solution. 
$\lambda=0$ is eigenvalue $\iff$ A not invertible

Finding eigenvalues
For $\lambda$ to be an eigenvalue and $v\neq 0$ such that
$$Av=\lambda v$$
$$AV-\lambda v=0$$
$$AV-\lambda Iv=0$$
$$(A-\lambda I)v=0$$
ie. need non-trivial solution to linear system
$$(A-\lambda I)\vec{x}-\vec{0}$$
Need coeff. matrix ($A-\lambda I$) to be non-invertible ie need
$$det(A-\lambda I)=0$$
The characteristic polynomial of a n\times n matrix is 
$$C_A(\lambda)=det(A-\lambda I)$$

Prop
$\lambda$ is a eigenvalue of $A$ $\iff$ $\lambda$ is root of the characteristic polynomial.

Example
A=\pmatrix{2&0&0\\1&2&-1\\1&3&-2}. find eigenvalues.

Sol
![[Screenshot 2024-12-01 at 3.12.17 PM.png]]
$=(2-\lambda)(\lambda^2-1)$
$=(2-\lambda)(\lambda+1)(\lambda-1)$
so eigenvalues are $2,1,-1$

notes
1. For $A$ $n\times n$, $C_A(\lambda)$ is polynomial of degree $n$.
2. A $n\times n$ has at most $n$ eigenvalues
3. $det(A-\lambda I)$ is long computation
4. Find roots of polynomial is hard. 


Finding eigenvectors
If \lambda eigenvalue, to find eigenvectors solve homo sys
$$(A-\lambda I) x=0$$
sols are the eigenvectors. 

If lambda eigenvalue of A, define the eigenspace E_\lambda by
E_\lambda = \{v\in\mathbb{R}^n|Av=\lambda v\} = set of solutions to (A-\lambda I)x=0

E_\lambda is a subspace since the sol set to a homo sys is subspace. 

Ex. For $A=\pmatrix{2&0&0\\1&2&-1\\1&3&-2}$ find a vasis for eigenspace
Sol. We already know 2,1,-2 from above
for \lambda =2 solve
$$\pmatrix{2-2&0&0\\1&2-2&-1\\1&3&-2-2}$$
Then we take that matrix along with the coef. matrix 0 and solve the lin system to find the vectors using EROs.


Observe
The vectors which form the eigenspace are linearly independent. You can then take the resulting eigenvectors and find the original matrix. We can geometrically better understand what the original transformation matrix does to a given vector. 