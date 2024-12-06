#math133 
A characteristic polynomial is a polynomial that is calculated from a square matrix and has the following properties: 
- [[Eigenvalues and eigenvectors|Eigenvalues]]: The roots of the characteristic polynomial are the eigenvalues of the [[matrix]]
- Matrix similarity: The characteristic polynomial is invariant under matrix similarity
- Coefficients: The characteristic polynomial's coefficients include the matrix's determinant and trace

Example:
$$A=\pmatrix{4&-1&6\\2&1&6\\2&-1&8}$$Find char. poly:
$$C_A=det(A-xI)$$
$$=|\matrix{4-x&-1&6\\2&1-x&6\\2&-1&8-x}|$$

$$=-(x-2)(x-9)(x-2)$$
*Therefore* eigenvalues are 2 and 9.

[[Eigenvector bases (diagonlisation)]]
