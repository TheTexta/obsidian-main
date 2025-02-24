#math133 
T:R^n->R^m a function
1. T called onto (or surjective) if Im(T)=R^m
2. T called one-to-one (or injective) if for all $u\neq v$. in r^n we have $T(u)\neq T(v)$ (no two inputs go to the same output). Equivalently if $T(u)=T(v)$ then $u=v$.
![[Screenshot 2024-11-29 at 12.31.17 PM.png]]

Example
T:R^3->R^2 def by T(x,y,z)=(x,y). 
T surjective? Im(T)=R^2, therefor true
T injective? No since $T(1,1,1)$ and $T(1,1,0)$ both equal $(1,1)$


Theorem (inj/sur)
Let $T:R^n->R^m$ be linear. Then
1. T surjective $\iff$ $rank (T)=m$
2. T injective $\iff$ $nullity(T)=0$ ($Ker(T)=\{\vec{0}\}$)

Ex: $TR^4->R^4$
$$T\pmatrix{x_1\\x_2\\x_3\\x_4}=\pmatrix{-x_1-2x_2+x_3\\x_1+2x_2\\3x_1+6x_2+x_3+x_4\\x_1+2x_2+x_3+x_4}$$
Is T injective? subjective?
Sol
Need $[T]$.

RREF of T gives us the rank which gives us the nullspace etc blah blah blah. 
rank T=3 neq 4 not sub. nullity =1 not 0 not inj. 

### Prop
Let T:R^n-R^m be lienar.
1. If $n>m$, T is not injective
2. If $n<m$ is not surjective

The proof is in the fact that $rank+nullity = n$. 


Function $f:R^n->R^m$ is called
- *bijective* if f is injective and surjective
- *invertible* if exists function $f^-1:R^m ->R^n$ such that $(f\cdot f^{0-1})(w)=w$, for all $w\in \mathbb{R}^m$ and $(f^{-1}\cdot f)(v)=v$

Fact: $f$ invertible $\iff$ $f$ bijective

Prop: Let $T:R^n->R^n$ then
1. T invertible $\iff$ standard matrix $[T]$ is invertible.
2. If T invertible, [T^{-1}]=[T]^{-1}
