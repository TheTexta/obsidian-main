#math133 
$A,B$ $n\times n$ called similar if $A=CBC^{-1}$ some $C$ $n\times n$ invertible. (C can be either side)
Prop: If $A=CBC^{-1}$ then
$$A^n=CB^nC^{-1}$$

##### Application: matrix powers
For $A=\pmatrix{0&-2\\1&3}$, find formula for $A^n$. Diagonalize $A=PDP^{-1}$, then $A^n=PD^nP^{-1}$ So find the Eigenvalues of A to find the eigenvectors and to then find the P matrix (matrix formed by placing eigenvectors as columns in the matrix).

$P=\pmatrix{-1&-2\\1&1}$, $D=\pmatrix{2&0\\0&1}$

$$P^-1=\frac{1}{1}\pmatrix{1&2\\-1&-1}$$

So

$$A^n=PD^nP^{-1}$$
$$=\pmatrix{2&0\\0&1}^nP^{-1}$$
$$=P\pmatrix{2^n&0\\0*1}\pmatrix{1&2\\-1&-1}$$
$$=\pmatrix{-1&-2\\1&1}\pmatrix{2^n&2\cdot 2^n\\-1&-1}$$
$$=\pmatrix{-2^n+2&-2^{n+1}+2\\2^n-1&2^{n+1}-1}$$


##### Prop
Let A,B be similar matrices. Then
1. $det(A)=det(B)$
2. $C_A(\lambda)=C_B(\lambda)$, some char. poly.
3. Same eigenvalues with same algebraic and geometric multiplicities


### How to change bases
Let B={vectors v to v_n} be bases of R^n. Each u\in R^n can be uniquely expressed as u=coefficients times vectors v.

Define the [[B-coordinate vector]] of u as $[u]_B=\pmatrix{c_1\\c_2\\...\\c_n}$