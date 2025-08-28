Def: $T:R^n-R^m$ linear, $[T]$ is $m\times n$ matrix
- kernel (or [[nullspace]]) of $T$ is $Ker(T)=\{\vec{u}\in R^n|T(u)=0\}$ ie sol set to homogeneous system $[T]x=0$
- nullity (T)=dim ker(T)
- Image of T is all $w\in R^m$ such that there is a vector in $R^n$ with $T(u)=w$ - ie all outputs. In matrix terms all vectors w such that $[T]x=w$ has a solution. if $[T]=[T(e_1),...,T(e_n)]$ then $[T]\pmatrix{x\\...\\x_n}=w$. Image (T)=column space of $T$ - $col[T]$
- The rank is the preserved dimensions and the nullity is the lost dimensions


Theorem (rank nullity theorem)
$T:R^n->R^m$ linear, then
rank(T)+nullity(T)=n where n is the number of columns