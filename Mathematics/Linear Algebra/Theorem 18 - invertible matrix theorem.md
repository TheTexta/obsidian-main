#math133 
Let $A$ $n\times n$ [[matrix]] the following statements are equivalent
1. A is [[Invertibles|invertible]] ($AB=I$ and $BA = I$ for some $B$)
2. The [[homogeneous system]] $A\vec{x}=\vec{0}$ has unique solution $\vec{x}=\vec{0}$
3. Row reduces to $I$
4. A can be written as a product of [[elementary matrices]]
5. For every [[vector]] $\vec{b}\in\mathbb{R}^n$, system $A\vec{x}=\vec{b}$ is [[consistent]] (in fact has unique solution)
6. [[Matrix rank|rank]]$(A)=n$ ie. rank is max
7. $AB=I$ for some $B$ $n\times n$
8. $CA=I$ for some $C$ $n\times n$
##### Proof of 1-4 equivalent
$1 => 2$: assume $A^{-1}$ exists.
Then 
$A\vec{x}=\vec{0}$
$AA^{-1}\vec{x}=A^{-1}\vec{0}$
$I\vec{x}=\vec{0}$ so $\vec{x}=\vec{0}$

$2=>3$: Assume $A\vec{x}=\vec{0}$ has unique solution $\vec{x}=\vec{0}$
$[A\vert{}\vec{0}]->[R\vert{}\vec{0}]$ where $R$ is [[reduced row echelon form|rref]] of $A$
if $R$ has zero row, [[free variables|free variable]] so inf many solutions. not possible. since inque sol. So all n row have leading 1 so R=I. A-> I by eros

3=>4: Prop 17.

4=>1: assume there exists elementary matrices such that $A=E_1...E_m$. but each $E_i$ invertible here so is A

### Application: [[Markov Chain Example]]

### Background
knowing when a matrix is invertible its really important to know later. *The most important theorem to know in the class*

Logic:
- $P=>Q$ - P [[implies]] Q
- Suppose we have many statements
	- 1. ....
	- 2. ....
	- n. ....
- we say the statements are equivalent if any one can be proved from any other one. 1 =>2, 2=>3, 3=>1, etc.
- must be either all true or all false.
- ![[Screenshot 2024-10-15 at 10.49.36 AM.png]]
