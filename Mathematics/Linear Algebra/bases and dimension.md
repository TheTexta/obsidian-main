#math133 
![[Screenshot 2024-11-27 at 10.44.37 AM.png]]

This plane is a 2d space. 

A basis is like the most simple version of a given span. A span containing only the most necesary vectors to build the span which are a subspace of a given vector space. 

Let U be a subspace of R^n. u_1,...,u_m \in U. We call these vectors a **basis** of U if
1. span{u_1,...,u_m}=U (enough vectors to create U)
2. Vectors are lin independent (no excess vectors)

Example
1. $\{e_1,...,e_n\}$ is a basis of R^n called the standard basis.


### Building a basis
if v_1,...,v_m are independent, and v_m+1 is not in span {v,...,v} then v indpenendent. Basically you have a span of given vectors and the next given vector cannot be built from that span then all the vectors including the next one are independent.

##### Building a basis 2
![[Screenshot 2024-11-27 at 11.08.53 AM.png]]
Take vectors and continuously add (checking for independence) to the span until they form the span. 

### Theorems relating to bases
#### Theorem 1
Let $U=span\{v_1,...,v_m\}$
1. $U$ has a basis of size $m$
2. every basis of $U$ contains same number of vectors (important)
3. Every independent set of vectors in $U$ has size less or equal to $m$. 

notation
If $X$ finite set. $|X|$ is the number of elements (cordiality) in $X$.

def
Let $U$ be a subspace of $R^n$ with bases $B$. The dimension of $U$ is number of vectors in $B$
$$dim (U) = |B|$$

If $u\neq 0$, dim span{u} =1 (all possible multiples of one vectors remain in one dimension)

For $U=\{\vec{0}\}$, which is subspace, empty set {} is basis, so dim{0}=0. 

#### Theorem 2
Let U be a subspace of R^n. Then
1. U has a finite basis. So, U=span {v_1,...,v_m} for some v's (every subspace is a span)
2. dim U \leq n
3. If I={vectors v} is independent. set of vectors in U, then
	1. |I|\leq dim U
	2. if span I \neq U, then I can be enlarged by adding new vector to form basis
4. if S={set of vectors u} is a set of vectors such that span S= U
	1. |S|\geq dim U
	2. If S is dependent we can remove some vectors from S to obtain a basis of U.


#### Theorem 3
Let U be a subspace of R^n, m = dim(U) and let X = {m vectors of v} (|X|=m=dim U). Then $$X \text{ indepedent} \iff\text{ span }X = U$$. basically If U is a valid subspace it will have independent vectors to form its span so if X is of the same dimensions as the subspace (exact number of vectors to form the subspace U) it will also only contain indendent vectors if the span of X = subspace U.

Problem
Let $u,v,w \in R^3$ all non zero mutually orthogonal. u\cdot v=0, u\cdot w=0, v\codt w=0. Show they are basis of R^3
![[Screenshot 2024-11-27 at 11.43.54 AM.png]]

Sol:
dim R^3=3. and 3 vectors (correct number for basis). we can show independent or span, other property from them 3. 
suppose
au+bv+cw=0
![[Screenshot 2024-11-27 at 11.46.16 AM.png]]

#### Theorem 4
Let $U,W$ subspace of $R^n$ with $U\leq W$. 
1. $dimU\leq dim W$
2. If dim are same then they are the same subspace $U=W$