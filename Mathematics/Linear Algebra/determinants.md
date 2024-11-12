#math133 

### Computing Determinants
def: for A $n\times n$ [[matrix]] define determinants $det(A)$ or $|A|$ as follows. Denote $A=[a_{ij}]$ and $A_{ij}^~ = (n-1)$ $\times$ $(n-1)$ obtained by removing row $i$, column $j$ of A. then,
1. If n=1, det ([a])=a
2. If $n\geq 2$, let $i$ be any of 1,2,...,n. 
	define $C_{ij}=(-1)^{i+j}det(A_{ij}^(~))$ called (i,j) cofactor. 
	then $det(A)=\sum_{j=1}^n a_{ij}c_{ij}(A)$
			 $=a_{ij}c_{ij}(A)+a_{in}c_{in}(A)$
			 Called cofactor expansion

![[determinant proof observation.png]]
###### Example 1
![[Screenshot 2024-10-15 at 12.41.37 PM.png]]
###### Example 2
![[Screenshot 2024-10-15 at 12.58.42 PM.png]]
##### Pro 18 - Property of computing a determinant
determinant does not depend on which row i is used and for each $j=1,2,...,n$  $det(A)=\sum_{i=1}^nA_{ij}c_{ij}(A)$

##### notation
$det(A)=|\matrix{a&b\\c&d}|$


### Properties
##### Properties of upper/lower [[Triangular Matrix|triangular matrices]]
if A triangular (upper or lower), $det(A)=$product of entrees on diagonal. det (I) = 1

###### Example
let $V=\pmatrix{1&a_1&a_1^2\\1&a_2&a_2^2\\1&a_3&a_3^2}$
find the det
$=|\matrix{1&a_1&a_1^2\\0&a_2-a_1&a_2^2-a_1^2\\0&a_3-a_1&a_3^2-a_1^2}|$
$=1\cdot |\matrix{a_2-a_1&a_2^2-a_1^2\\a_3-a_1&a_3^2-a_1^2}|$
![[Screenshot 2024-10-15 at 1.48.08 PM.png]]
factor out
$=(a_2-a_1)(a_3-a_1)\cdot |\matrix{1&a_2-a_1\\1&a_3-a_1}|$


##### Properties of square determinants
let $A$ $n\times n$ matrix
1. If $A$ has a row / column of all zeros the $det(A)$ must be zero
2. If $A$ has two identical rows / columns the $det(A)$ must be zero
3. $det(cA)$ $=$ $c^n$ $\cdot$ det$(A)$ - each operation mult determinant by $c$.
4. If matrix block triangular form where each $B_i$ is a square block $det(A) = det(B_1)\cdot ... \cdot det(B_k)$![[Screenshot 2024-11-11 at 4.08.50 PM.png]]

##### Determinants and [[Elementary Matrices]]
Let $E$ be an [[elementary matrices|elementary matrix]]. Then
1. $det(E)\neq 0$, in fact if [[Elementary Row Operation|ERO]] used to create $E$ was
	1. $R_i$ -> $cR_i$, then $det(E) = c$
	2. $R_i$ -> $R_i + cR_j$, then $det(E)=1$
	3. $R_i$ <-> $R_j$, then $det(E) = -1$
2. If $A$ $n\times n$ matrix, then
	1. $det(EA) = det(E)\cdot det(A)$

##### [[Theorem 23 - Determinants and Invertibles]]
Let $A$ $n\times n$ then,
$A$ invertible $\iff$ $det(A) \neq 0$

##### [[Theorem 24 - Splitting determinants]] 
Let $A,B$ $n\times n$ then,
$det(AB)=det(A)+det(B)$

