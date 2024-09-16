#math133 
The transpose of a $m \times n$ [[matrix]] $A$ is the $n \times m$ matrix $A^T$ whose $(i,j)$ entry is the $(j,i)$ entry of A.
$A^T = [a_{ji}]$

#### Properties of Transpose
1. $(A^T)^T=A$
2. $(cA)^T=c(A^T)$
3. $(A+B)^T=A^T+B^T$

#### Example
$A=\pmatrix{1&2&3\\4&5&6}\quad\quad A^T=\pmatrix{1&4\\2&5\\3&6}$ 

The rows become columns - a reflection of the line from top left to bottom right.

###### Problem
Let $A$ be $n \times n$ [[matrix]]. Show $B=A+A^T$ is [[symmetric matrix|symmetric]]
*Solution*
$B^T=(A+A^T)^T$
$\quad = A^T+A$
$\quad =A+A^T$
$\quad=B$ therefore $B$ is [[symmetric matrix|symmetric]]