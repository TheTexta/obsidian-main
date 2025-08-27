#math133 
$X=\{u_1,u_2,...,u_m\}\subseteq R^n$
The span of X, Span(X), is the set of all linear combinations of vectors of X, i.e.
Span X = $\{c_1u_1+...+c_mu_m|c\in R\}$ 

If $X=\{\}$ (no vectors, $X$ is an empty set), define
Span $X$ = $\{\vec{0}\}$


![[Screenshot 2024-11-26 at 4.34.38 PM.png]]
The span of a R^3 vector is a line through 0,0,0

### Span of two vectors in R^2
Will be R^2 so long as the two vectors are not linearly dependent. (non zero and non-parallel).
![[Screenshot 2024-11-26 at 4.37.45 PM.png]]
![[Screenshot 2024-11-26 at 4.40.28 PM.png]]
Since u,v not zeor not parallel rank A^T=2, A^T is inv so exists a sol for every c1,c2.

### Span of two vectors in $\mathbb{R}^3$
let $u,v$ $\in \mathbb{R}^3$ non-zero, non-parallel. 

The span of the two vectors is the plane through the origin with the normal vector $u\times v$

### Theorem
let $U$=span $\{u,u_2,..,u_m\}$, $u\inR^n$ for all $i$. then
1. $U$ is a subspace (every span is a subspace)
2. $u_i$ $\in U$ for all $i$
3. If W is a subspace of $R^n$ and $u_i\in W$ for all i, then span $U=\{u_1,...,u_m\}\subseteq W$


Let U be a subspace of R^n. If U=span{vectors u}. we say that U is spanned by vectors vectors u. 
1. R^3 = span $\{e_1,e_2,e_3\}$ since if $u=\pmatrix{a\\b\\c}\in R^3$ then $\pmatrix{a\\b\\c}=a\pmatrix{1\\0\\0}+b\pmatrix{0\\1\\0}+c\pmatrix{0\\0\\1}$
2. R^n is a subspace of R^n
##### Example of proving vectors span a subspace
![[Screenshot 2024-11-26 at 6.07.21 PM.png]]![[Screenshot 2024-11-26 at 6.08.05 PM.png]]
Since A is inv. so sol is unique for all $u=\pmatrix{a\\b\\c}$

