13. computing determinants
##### def: for A $n\times n$ [[matrix]] define determinants $det(A)$ or $|A|$ as follows.
Denote $A=[a_{ij}]$ and $A_{ij}^~ = (n-1)$ $\times$ $(n-1)$ obtained by removing row i, column j of A.
then,
1. If n=1, det ([a])=a
2. If $n\geq 2$, let $i$ be any of 1,2,...,n. 
	define $C_{ij}=(-1)^{i+j}det(A_{ij}^(~))$ called (i,j) cofactor. 
	then $det(A)=\sum_{j=1}^n a_{ij}c_{ij}(A)$
			 $=a_{ij}c_{ij}(A)+a_{in}c_{in}(A)$
			 Called cofactor expansion

![[determinant proof observation.png]]
##### Example 1
![[Screenshot 2024-10-15 at 12.41.37 PM.png]]
##### Example 2
![[Screenshot 2024-10-15 at 12.58.42 PM.png]]
##### Pro 18
determinant does not depend on which row i is used and for each $j=1,2,...,n$  $det(A)=\sum_{i=1}^nA_{ij}c_{ij}(A)$

##### notation
$det(A)=|\matrix{a&b\\c&d}|$


### Some shortcuts
##### Def upper triangular
![[Screenshot 2024-10-15 at 1.35.39 PM.png]]
i.e. $a_{ij}=0$ for all $i>j$. 

Strictly upper triangular if
$a_{ij}=0$ for all $i\geq j$

##### prop 20
if A triangular (upper or lower), det(A)=product of entrees on diagonal. det (I) = 1

##### Example
let $V=\pmatrix{1&a_1&a_1^2\\1&a_2&a_2^2\\1&a_3&a_3^2}$
find the det
$=|\matrix{1&a_1&a_1^2\\0&a_2-a_1&a_2^2-a_1^2\\0&a_3-a_1&a_3^2-a_1^2}|$
$=1\cdot |\matrix{a_2-a_1&a_2^2-a_1^2\\a_3-a_1&a_3^2-a_1^2}|$
![[Screenshot 2024-10-15 at 1.48.08 PM.png]]
factor out
$=(a_2-a_1)(a_3-a_1)\cdot |\matrix{1&a_2-a_1\\1&a_3-a_1}|$

##### Prop
- let $A$ $n\times n$ [[matrix]]
	- If $A$ has a row or column of all $0$, [[determinants|det]](A) = 0. (co)