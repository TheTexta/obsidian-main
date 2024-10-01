#math133 
### Overview
##### Def
Given $S:R^n->R^m$, $T:R^m->R^p$ transformations, define the *composition* $T\cdot S:R^n->R^p$ by, for each $v\in R^n$,

$(T\cdot S)(\vec{v})=T(S(\vec{v}))$
![[Screenshot 2024-09-22 at 3.44.28 AM.png]]

##### Example
A=((1,2)(0,-3)), B=((2,1),(1,-1))
Find formulas for $T_A \cdot T_B:R^2->r^2$ and $T_B \cdot T_A:R^2->r^2$

So
$(T_a \cdot T_b)(x,y)=T_A(T_B(x,y))=T_A((2,1),(1,-1))(x,y)=T_A(2x+y,x-y)$
$=((1,2)(0,-3))(2x+y,x-y)=(2x+y+2x-2y,0-3x+3y)=(4x-y,-3x+3y)$

If we set $c=((4,-1),(-3,3))$ then $T_c(x,y)=(4x-y,-3x+3y)$.

we will define the product A B (x) = Cx as C

$A(B\vec{x})=A([b_1, b_2] \pmatrix{x\\y})$
	   $= A(xb+yb)$
	   $=A(x\vec{b}_1+y\vec{b}_2)$
	   $=x(A\vec{b}_1)+y(A\vec{b}_2)$ 
	   $=[\matrix{A\vec{b}_1 & A\vec{b}_2}]\pmatrix{x\\y}$
	   $=A\cdot B\pmatrix{x\\y}$ 

### Properties of matrix multiplication
Let A,B,C matrices of appropriate sizes
1. A $m \times n$
	1. $AI_n = A$
	2. $I_nA = A$
	Proof
	$AI_n=A[\matrix{e_1&e_2&...&e_n}]$
		$=[\matrix{Ae_1&Ae_2&...&Ae_n}]$
		$=A$
2. $(AB)C=A(BC)$ - The [[associative rule]]
3. $A(B+C) = AB+AC$ (not the same as $BA+CA$!!)
   $(B+C)A=BC+CA$
4. For any scalar $k\in\mathbb{R}$
	1. $k(AB) = (kA)B = A(kB)$

##### Examples
$A,B$, $n\times n$ matrices
$(2A-3B)(-A+4B)$
$= -2AA+(2A)(4B)+3BA+(-3B)(4B)$
$= -2A^2+8AB+3BA-12B^2$ ($AB$ and $BA$ not same!! - not [[commutative]])

