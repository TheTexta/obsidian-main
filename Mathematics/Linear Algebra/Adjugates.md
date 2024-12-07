#math133 
Adjugates formula for A inverse
Let $A$ $n\times n$. let $C_{ij}$ be the $C_{ij}$ cofactor ie. $C_{ij}=(-1)^{i+j}det(\hat{A_{ij}})$
The adjugate of $A$ (also called classical adjugate)
$$adj(A)=\pmatrix{C_{11}&C_{12}&...&C_{1n}\\...&...&...&...\\C_{n1}&...&...&C_{nn}}^T$$

##### Example for $2\times 2$ matrix
Ex for $A=\pmatrix{a&b\\c&d}$
$adj(A)=\pmatrix{C_{11}&C_{12}\\C_{21}&C_{22}}=\pmatrix{d&-b\\-c&a}$


### [[Formula for A inverse using adjugates]]
Let $A$ $n\times n$. then
$A(adj(A))=det(A)I$
hence
$A^{-1}=\frac{1}{det(A)}\cdot adj(A)$
(if A invertible)


##### Example 3x3 inverse using adjugates
$$

A \, \text{adj}(A) = 
\begin{pmatrix}
a_{11} & a_{12} & a_{13} \\
a_{21} & a_{22} & a_{23} \\
a_{31} & a_{32} & a_{33} \\
\end{pmatrix}
\begin{pmatrix}
C_{11} & C_{12} & C_{13} \\
C_{21} & C_{22} & C_{23} \\
C_{31} & C_{32} & C_{33} \\
\end{pmatrix}
$$
$$=\pmatrix{det(A)&0&0\\0&det(A)&0\\0&0&det(A)}$$
