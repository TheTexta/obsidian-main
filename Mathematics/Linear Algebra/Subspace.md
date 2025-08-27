#math133 
A subset of $\mathbb{R}^n$ is a collection ("set") of vectors $X$ each of which comes from $\mathbb{R}^n$
Write $$X\subseteq R^n$$ and if u is a vector in X, write
$$u\in X$$
##### Example - not subspace
$$X=\{\pmatrix{a\\b}\in\mathbb{R}^2|a^2+b^2\leq 1\}$$
X is a collection (subset of $\mathbb{R}^2$) of vectors $\pmatrix{a\\b}$ such that $a^2+b^2\leq1$
##### Example 2 - subspace
$$L=\{\pmatrix{a\\b}\in\mathbb{R}^2|a=b\}$$

Let $U\subseteq \mathbb{R}^n$. then $U$ is called a subspace of $R^n$ if the following hold:
1. $\vec{0}\in U$
2. If $u,v \in U$, then $u+v \in U$ (closure under addition)
3. If $u \in U$ and $c\in R$, then $cu\in U$. (closure under scalar multiplication)
If all 3 hold. write $U\subseteq R^n$

Every plane where the origin is zero is a subspace.

A line which goes through the origin is a subspace.

To verify a set is not a subspace just verify one of the failing conditions is indeed false. 

### Theorem
$$\text{Let } A \text{ be an } m \times n \text{ matrix, } \vec{b} \in \mathbb{R}^m, \text{ consider}
$$
$$\text{Lin. system } A \vec{x} = \vec{b}. \text{ Let }
S = \{\vec{u} \in \mathbb{R}^n \mid A \vec{u} = \vec{b}\}
\quad \text{[ie. sol set to } A \vec{x} = \vec{b} \text{]}.
$$
$$\text{Then } S \text{ is a subspace } \iff \vec{b} = \vec{0}, \text{ i.e. homogeneous system}.
$$

##### Example using homogenous system proof
![[Screenshot 2024-11-26 at 3.50.24 PM.png]]