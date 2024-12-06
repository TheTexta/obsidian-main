#math133 
Def $A$ $n\times n$ matrix called diagonalisable if there is a basis $v$ of $R^n$ where all $v_i$ are eigenvectors of A. 

Ex
$TR^3-R^3$ rotation about z-axis by $\pi$.
$T(e_1)=-e_1$
$T(e_2)=-e_1$
$T(e_3)=e_3$

T is diagonalisable since {$e_1,e_2,e_3$} is a basis $R^3$ compared eigenvectors of T.
TLDR if there are enough eigenvectors to make up a basis of a matrix then the matrix is diagonalisable.

if dterminant is greater then zero than the matrix is linearly independent. 

##### Diagonalisation in matrix terms
A $n\times n$ matrix, assume there is bases v-v_n of R^n where Av_i=\lambda_iv_i, ie. v_i eigenvoectors with eigenvalue \lambda_i.
Set P=\[v_1,v_2,...,v_n\]=matrix of eigenveotr of A
Since v-v_n ind P invertible.
AP=A\[v_1,v_2,...,v_n\]
=\[lambdav,...,\lambda_n v_n\]

A=PDP^-1
Transforming A into a diagonalisable matrix. 
![[Screenshot 2024-12-05 at 4.20.33 PM.png]]
If v vectors is a basis of R^n where Av=\lambda v, then A=PDP^-1 with P=vectors and D=\pmatirx{lambeda ...} along each row in 

Ex.
For A=\pmatrix{4&-1&6\\2&1&6\\2&-1&8} find P,D where A=PDP^-1.
Find C_A(T)=-(x-2)^2(x-9) from so eigenvalues are 2,9

For eigenvalue 2: Solve (A-2I)\vec{x}=\vec{0}
![[Screenshot 2024-12-05 at 4.24.39 PM.png]]

$E_2=span{\pmatrix{1\\2\\0},\pmatrix{-3\\0\\1}}$
For eigenvalue=9
![[Screenshot 2024-12-05 at 4.30.30 PM.png]]

