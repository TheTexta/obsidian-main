#math133 
The vectors which substitute x to satisfy the equation Ax=0 for a given matrix. The nullspace is a subspace. 

Let A $m\times n$ matrix. the nullspace of $A$ is solution set to $Ax=0$ ie $null(A)=\{u\in R^n|Au=0\}$
It is a subspace. if l=# free variables in Ax=0, and general solution obtained Gaussian elimination is x=tv +... t_lv_l then vectors v called basic solution to Ax=0 and l=n-r

The dimension of null(A) is called the nullity of A.


### Theorem - Rank nullity theorem
A m \times n, r=rank(A)
1. the n-r basic solutions form bases of null(A) hence nullity (A)=n-r
2. n=rank(A)+nullity(A) (r+(n-r)=n)

#### Example
$$A=\pmatrix{5 & 2 & 3 & 1 \\ 0 & -1 & -4 & 2 \\ 2 & 1 & 2 & 0 \\ 1 & 1 & 3 & -1}$$
Find rank and nullity of A, and vases for im(A) and null(A)

sol
$$R=\pmatrix{1&0&-1&1\\0&1&4&-2\\0&0&0&0\\0&0&0&0}$$
rank (A)=2, by then nullity(A)=4-2=2 (\# of columns - \# of leading ones)

for im(A), bases given by columns 1,2 of A ie. (image is the column space - span of the columns)
$$\pmatrix{5\\0\\2\\1},\pmatrix{2\\-1\\1\\1}$$
for nul(A), solve Ax=0, so
$$\matrix{x_1&=&s-t\\x_2&=&-4s+2t\\x_3&=&s\\x_4&=&t}$$
$$\vec{x}=s\pmatrix{1\\-4\\1\\0}+t\pmatrix{-1\\2\\0\\1}$$
basic solution ^ form the basis of nul(A) (this solutions forms the span of the vectors which allow for Ax=0)