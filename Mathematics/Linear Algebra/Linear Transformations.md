#math133 
A function T:R^n->R^m is a linear transformation (function and transformation are the same just transformation is the word used in linear algebra) if
1. $T(u+v)=T(u)+T(v)$ for all u,v\inR^n- property puts restrictions on what the transformations can do
2. $T(cu)=cT(u)$ for all $u\in R^n$,$c\in R$

### Properties
Let T:R^n->R^m be linear transformation
1. $T(\vec{0}_n)=\vec{0}_m$ - really quick way to check if a lin trans is valid.
2. $T(a_1v_1,...,a_n,v_n)=a_1T(v_1)+...+a_nT(v_n)$

### Theorem (T determined by values on bases)
let v_1,...,v_n basis of R^n, w_1,...,w_m of R^m any vectors. THen there exists exactly one linear transformation T:R^n->R^m that satisfies T(v_i)=w_i all i=1,...,n
Further if v\in R^n and we express v=a_1v_1+...+a_nv_n then
T(v)=a_1w_1+...+a_nw_n

##### Example
suppose T:R^3->R^2. is linear and T(1\\1\\0)=(1\\2),T(0\\1\\1)=(-1\\1),T(1\\0\\1)=(2\\1) find T(1\\2\\-1).

Sol
(1\\1\\0),(0\\1\\1),(1\\0\\1) form basis R^3. We can write (1\\2\\-1) in terms of basis, (1\\2\\-1)=a(1\\1\\0)+b(0\\1\\1)+ (1\\0\\1)
Solve obtaine whatever for a,b,c - sub in the known tranform sol then add together to find the new transform.

### Examples
1.
T:R^2->R^3
$T(\pmatrix{x\\y})=\pmatrix{x+3\\yx\\e^x}$ is not linear since
$T(3\pmatrix{1\\2})\neq 3T(\pmatrix{1\\2})$


2.
If A m\times n, T_A:R^n->R^m defined by 
$T_A(x)=Ax$
is linear since
![[Screenshot 2024-11-28 at 1.05.07 PM.png]]

3.
Let R:R^2->R^2 be rotation counter-clockwise by \Theta about 0,0. It is linear tranform

4.
![[Screenshot 2024-11-28 at 1.21.36 PM.png]]