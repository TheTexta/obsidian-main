- Solving augmented matrixes through [[Elementary Row Operations]]
- Learning about [[Row Echelon Form]] and [[reduced row echelon form]].
- If a [[matrix]] row has all zero coefficients and a nonzero constant the [[system of linear equations|system]] is inconsistent. 
- A system can be consistent and have infinitely many solutions
- Verifying systems
- Parametric form for solutions. 
- An all zero row (constants and coefficients) implies redundancy / intersection
- If a solution includes a variable equalling another eg. $y=y$ then the solution is best written in parametric form (subbing in $y=t$).
- Solution to the system $x+2-z=1$, $2x+4y-z=8$ and $4x+3y-5z=10$ is $(5-2t,t,2)$ where $t\in \mathbb{R}$ or in [[parametric functions|parametric form]]:
		$x=5-2t$
		$y=t$
		$z=2$
- Non leading variables are called [[free variables]]. We rename the free variables and rewrite the equation in terms of these variables to create parameters. 

$$
\begin{pmatrix}  
1 & 0 & 2 & 0 &-2 &|+3\\  
0 & 1 & 3 & 0 &-1 &|+4\\
0 & 0 & 0 & 1 & 1 &|-2\\
\end{pmatrix}
$$
Column 3 and 5 contain [[free variables]] the rest contain [[leading variables]].

$x_1=3-2x_3+2x_5$
$x_2=y-3x_3+x_5$
$x_4=-2-x_5$
rename $x_3=s$ and $x_5=t$

Writing now in [[parametric functions|parametric form]]:
$x_1=3-2s+2t$
$x_2=y-3s+t$
$x_3=s$
$x_4=-2-t$
$x_5=t$