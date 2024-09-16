#math133 
If you do enough [[Elementary Row Operations|ERO]] you will end up with the same [[Row Echelon Form|REF]]. every matrix is row equivalent to a unique matrix in [[reduced row echelon form|RREF]].

Row Reduction algorithm
- [[Gauss Jordan Elimination]] (Gaussian elimination)
	- if all entries zero stop the algorithm
	- locate first nonzero leftmost column. take the row with the nonzero leftmost column and swap it for the top row and make it a one coefficient
	- get rid of all subsequent numbers in the same column using that leading one
	- Repeat steps 1 and 2 (ignoring top row)
	- This produces a [[row echelon form|REF]]
	- get [[reduced row echelon form|RREF]] by using each leading one (starting with rightmost) to get rid of all entries above

[[Matrix rank]] - every matrix has a rank. The rank cannot be greater then the number of rows/columns

Example
$$\begin{pmatrix}  
1 & 4 & |8\\  
0 & 0 & |c  
\end{pmatrix}$$
If $c\ne 0$ [[inconsistent]] and no solution
if $c=0$ [[Matrix rank|rank]] is 1

[[free variables]] $=$ variables $-$ [[Matrix rank|rank]]

Theorem 3 ([[number of solutions of a linear system]])
Consider linear system with n variables, m equations. suppose we find RREF of augmented matrix, it has rank r. 
1. if the last column contains a leading one system is inconsistent.
2. assume system is consistent
	- if $r=n$, no free variables and hence only one solution.
	- If r<n, there are n-r free variables hence infinitely many solutions

A system is called [[homogeneous system|homogeneous]] if all constant terms are zero. they cant be inconsistent they have to be consistent and the solution is called a [[trivial solution]]. 

Theorem 4 - [[homogenous system theorem]]
If we have a [[homogeneous system]]
1. always consistent
2. if only solution it is trivial solution
3. if more variables tan equations, infinitely many solutions

Problem
$-x +3y +2z=-8$
$x     +z=2$
$3x+3y+a=b$
For which $a,b$ do we get $0, 1, \infty$ many solutions?

#### Matrix Algebra
Addition, scalar multiplication and transpose

let $A$ be an $m$ x $n$ [[matrix]]
[[IJEntry|Entry]] in each row $i$, column $j$ called $(i,j)$ entry of the [[matrix]], usually denoted $a_{ij}$

###### Example of Matrix
$$A=\begin{pmatrix}  
a_{11} & a_{11} & ... & a_{1n}\\  
a_{11} & a_{11} & ... & a_{2n}\\
\vdotswithin{} \\
a_{m1} & a_{m2} & ... & a_{mn}
\end{pmatrix}$$

Another format:
$A=[a_{ij}]$

###### Other forms
A [[matrix]] denoted by $m$ x $1$ is a [[column vector]]

A 1 x n matrix is a [[row vector]]

A real number $c\in \real$ is also called a [[scalar]]

[[equal matrixes]]: two matrixes equal if same size with same entries.