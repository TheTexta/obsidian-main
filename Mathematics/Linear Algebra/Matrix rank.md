#math133 
for any [[matrix]] the number of leading ones in the [[reduced row echelon form|RREF]] is the rank. The rank cannot be greater then the number of rows/columns. keep in mind these questions can look easier then they actuall are like question 1 in the example

For matrix A if it has 4 leading ones then the rank(A)=4.

[[free variables]] $=$ variables $-$ [[Matrix rank|rank]]

### Example
![[rank question example.png]]

### Lemma
Let A-> B by [[Elementary Row Operation|ERO]]. Then
1. row(A)=row(B) - ie [[Elementary Row Operation|EROs]] don't change the [[span]] of the rows
2. EROs preserve relations amongst the columns

Proof.
1. Swap rows mult by constant doesn't change span. Suppose $r_i$->$r_i +cr_j$ new row in [[span]] of original rows and we can recover $r_i$ with the reverse op. so [[span]] doesn't change


Theorem (Rank Theorem)
Let A $m\times n$, r=rank(A), R=rref(A). then
1. The non-zero rows of R form basis of row(A). Hence, $r=dim[row A]$
2. If leading 1s of R are in columns i_1,...,i_r (r=rank (A)) then columns form basis of col(A). Hence r=dim(col(A))
3. Row and col space have same dimensions rank(A)=dim(row(A))=dim(col(A))

*Problem*
let $v_1=\pmatrix{1\\2\\3\\-1}, v_2=\pmatrix{-1\\3\\1\\1}, v_3=\pmatrix{3\\-4\\1\\-3}, v_4=\pmatrix{1\\7\\7\\-1}, v_5=\pmatrix{2\\2\\-1\\-1}$
set $V=span\{v_1,...,v_5\}$ (in $\mathbb{R}^4$)

Find [[bases and dimension|dim]] $V$ and [[bases and dimension|basis]] for $V$. (dim - min number of vectors to form the span, basis-specific minimum vectors to form the span)

Sol #1: via a row space
let $A=\pmatrix{v_1\\v_2\\v_3\\v_4\\v_5}$, $$A=\pmatrix{1 & 2 & 3 & -1 \\-1 & 3 & 1 & 1 \\3 & -4 & 1 & -3 \\1 & 7 & 7 & -1 \\2 & 2 & -1 & -1 \\}$$ so V=row(A). row-reduce A
$$A=\pmatrix{1 & 0 & 0 & -\dfrac{20}{27} \\
0 & 1 & 0 & \dfrac{4}{27} \\
0 & 0 & 0 & 0 \\
0 & 0 & 0 & 0 \\
0 & 0 & 1 & -\dfrac{5}{27} \\}$$
so we get the vectors
$$\begin{pmatrix}1\\0\\0\\ -\dfrac{20}{27} \end{pmatrix},\quad \begin{pmatrix}0\\1\\0\\ \dfrac{4}{27} \end{pmatrix},\quad \begin{pmatrix}0\\0\\1\\ -\dfrac{5}{27} \end{pmatrix}
$$
as the basis of the span of V, where the dimension comes to be 3. 

SOL 2:
via a column space
B=\[vectors v\]
![[Screenshot 2024-11-28 at 12.18.23 PM.png]]
can conclude v_1,v_2,v_5 form basis of col B =V 

##### Corollary
1. rank(A^T)=rank(A)
2. rank(AB)\leq rank(A) or rank(B)

