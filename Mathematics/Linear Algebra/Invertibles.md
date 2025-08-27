#math133 
### Algorithm for $A^{-1}$
Row reduce $[A:I]$ to $[R:B]$, $R=rref(A)$
1. if $R=I$, conclude $A$ is invertible and $B=A^{-1}$
2. If $R\neq I$, then $A$ not invertible.

want same for [[linear systems|linear system]] $A\vec{x}=\vec{b}$

##### Idea for finding $A^{-1}$
Let $A$ $3\times 3$, want to find $A^{-1}$.
Set
$$A^{-1}=\pmatrix{x_{11}&x_{12}&x_{13}\\x_{21}&x_{22}&x_{23}\\x_{31}&x_{32}&x_{33}}=[\matrix{\vec{z}_1&\vec{z}_2&\vec{z}_3}]$$
$$AA^{-1}=I$$
$$A[\matrix{\vec{z}_1&\vec{z}_2&\vec{z}_3}]=[\matrix{\vec{e}_1&\vec{e}_2&\vec{e}_3}]$$
$$[\matrix{A\vec{z}_1&A\vec{z}_2&A\vec{z}_3}]=[\matrix{\vec{e}_1&\vec{e}_2&\vec{e}_3}]$$
i.e.
$$A\vec{z}_1=\vec{e}_1$$
$$A\vec{z}_2=\vec{e}_2$$
$$A\vec{z}_3=\vec{e}_3$$
Which really results in 3 [[linear systems|linear systems]]
$$[A\:\vdots\matrix{1\\0\\0}],[A\:\vdots\matrix{0\\1\\0}],[A\:\vdots\matrix{0\\0\\1}]$$
Solutions equate to columns 1,2 and 3 respectably. 
If $A$ invertible, [[Matrix rank|rank]]$(A)=3$ - proof later.
hence [[reduced row echelon form|rref]](A) = [[identity matrix]]. When we solve $[A\:\vdots\matrix{1\\0\\0}]$, get $\pmatrix{1&0&0&\vdots&a\\0&1&0&\vdots&b\\0&0&1&\vdots&c}$. i.e. $\vec{x}_{11}=a,\vec{x}_{21}=b,\vec{x}_{31}=c$. Solve $[A\:\vdots\matrix{0\\1\\0}],[A\:\vdots\matrix{0\\0\\1}]$ with the same [[Elementary Row Operation|ERO]] as the first. therefor it makes more sense to solve all 3 simultaneously. $\pmatrix{A&\vdots&\matrix{1&0&0\\0&1&0\\0&0&1}} = \text{ruduced} = \pmatrix{I&\vdots&A^{-1}}$. 

###### Example
$3x=5$
$(3^{-1})3x=3^{-1}\cdot 5$
$1x=3^{-1}\cdot 5$
$x=3^{-1}\cdot 5$



##### Def
A $m\times n$. Say $A$ is invertible if there is [[matrix]] $B$, also $m\times n$ such that $AB=I_n$ and $BA=I_n$. Only one inverse can exist.
##### Proposition
Let A B C be m x n matrices
1. If $AB=I$, $BA=I$ and $AC=I$, $CA=I$ then $B=C$. Hence inverse matrix is unique, write $A^{-1}$
2. $AB=I \iff BA=I$

##### Proof
1. We have:        $AB=I$
			$C(AB)=CI$
			$(CA)B=C$
			   $IB=C$
			    $B=C$


### Properties of Inverses
1. $I^{-1}=I$ - of $II=I$.
2. If A invertible A^{-1} also invertible. $(A^{-1})^{-1}=A$
$$A^{-1}A=I$$
3. *very important*. If A, B both n\times n invertible then AB is invertible and
$$(AB)^{-1}=B^{-1}A^{-1}$$
*proof*: both $A^{-1},B^{-1}$ exist so $B^{-1}A^{-1}$ exists
$$AB(B^{-1}A^{-1})$$
$$=A(BB^{-1})A^{-1}$$
$$=AIA^{-1}$$
$$=AA^{-1}$$
$$=I$$
4. If $A_1, A_2, ..., A_k$ all $n\times n$ invertible then $A_1,A_2,...,A_k$ is invertible and
$$\pmatrix{A_1&A_2&...&A_k}^{-1}=A_k^{-1},A_k^{-1},...,A_2^{-1}$$
5. If $A$ invertible, $m\geq 1$ (int) then 
$$A^m \text{ is invertible and } (A^m)^{-1}=(A^{-1})^m$$
proof:
$$\text{By }(4) \text{ set }A_i=A \text{ for }i=1,2,...,m \text{ so }$$
$$(A^m)^{-1}=\pmatrix{A_1&A_2&...&A_m}^{-1}$$
$$=A_m^{-1} A_{m-2}^{-1}...A_{2}^{-1}A_{1}^{-1}$$
$$=A^{-1}A^{-1}...A^{-1}A^{-1}$$$$=(A^{-1})^m.$$
6. If $A$ invertible and $c\in \mathbb{R}$, $c\neq 0$ then $cA$ is invertible and
$$(cA)^{-1}=\frac{1}{c}A^{-1}$$
proof: since $c\neq 0$, $\frac{1}{c}$ exists so $\frac{1}{c}A^{-1}$ exists then
$$(cA)(\frac{1}{c}A^{-1})=(c\cdot \frac{1}{c})(AA^{-1})$$
$$=I$$
7. If $A$ invertible $A^T$ also invertible and 
$$(A^T)^{-1}=(A^{-1})^T$$
Proof: verify
$$A^T\cdot (A^{-1})^T=(A^{-1}A)^T$$
$$=I^T$$
$$I$$