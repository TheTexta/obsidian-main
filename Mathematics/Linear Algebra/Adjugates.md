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

### Polynomial Interpretation
![[polynomial interpretation.png]]
can find polynomial $f(x)$ such that $f(x_i)=y_i$ for all $i$. this can be done with polynomial of degree $n$ where $n=i-1$. 
$$\begin{pmatrix} 1 & x_0 & x_0^2 & \dots & x_0^n \\ 1 & x_1 & x_1^2 & \dots & x_1^n \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 1 & x_n & x_n^2 & \dots & x_n^n \\ \end{pmatrix} \begin{pmatrix} a_0 \\ a_1 \\ a_2 \\ \vdots \\ a_n \\ \end{pmatrix} = \begin{pmatrix} y_0 \\ y_1 \\ \vdots \\ y_n \\ \end{pmatrix}$$
Sys of $n+1$ equations is $n+1$ variables
$$V=\begin{pmatrix} 1 & x_0 & x_0^2 & \dots & x_0^n \\ 1 & x_1 & x_1^2 & \dots & x_1^n \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 1 & x_n & x_n^2 & \dots & x_n^n \\ \end{pmatrix}$$
This is a [[vandermonde matrix]]
$det(V)=\text{produce of all factors of form } (x_i-x_j) \text{ where } i>j$
$det(V)=(x_2 - x_1)(x_3 - x_1)(x_3 - x_2) \dots$
$= \prod_{\substack{n \geq i > j \geq 1}} (x_i - x_j)$
we have all $x_i$ distinct, hence $det(V)\neq 0$. hence $V$ [[invertibles|invertible]] so [[linear systems|system]] has unique solution