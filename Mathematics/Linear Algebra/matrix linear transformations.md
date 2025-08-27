#math133 

##### example
let $A=\pmatrix{2&0\\0&3}$. if $\vec{v}=\pmatrix{x\\y}$ then $Av=\pmatrix{2&0\\0&3}\pmatrix{x\\y}=\pmatrix{2x\\3y}$ think of $x,y$ as the input and $2x,3y$ as the output. the matrix is really a function in this context. a way of encoding what to do to the input. 

##### Def
A transformation (or function) from R^n to R^m is a rule that given a T, that given a vector v\inR^n (input) gives a vector called T(v) (output). write $T:R^n->r^m$, call $R^n$ domain, $R^m$ called the codomain (eg take a 2d dim vector as input and a 3d vector as output). 

##### Def: A matrix / linear transformation
Every $m\times n$ [[matrix]] $A$ defines a transformation $T_A$: $T_A(v)=Av$

##### Example
$A=\pmatrix{1&2&3\\4&5&6}$, so $T_a:R^3->r^2$ is defined by $T_A\pmatrix{x\\y\\z}=\pmatrix{1&2&3\\4&5&6}\pmatrix{x\\y\\z}$
$=\pmatrix{x+2y+3z\\4z+5y+6z}$

##### Some specific matrix transforms
1. A=((1,0)(0,-1)) then t_a:R^2->r^2, t_A(x,y)=((1,0)(0,-1))(x,y)=(x,-y). This reflects the vector over the x-axis. 
2. A=((c,0),(0,1)) is called an x-expansion if c>1 and an x-contraction if 0<c<1
3. Same as above can be applied for y by switching the c and 1
4. A=((1,c),(0,1)) is called a x-shear, changing shear by a factor of y and c.
5. same as above but swapped is a y shear.

##### Two special matrix transformations
1. [[identity matrix|Identity matrix]] $I_n$ defines *identity transformation* $T_{I_n}:R^n->R^n$
		 $T_{I_n}(\vec{v})=I_n\vec{v}=\vec{v}$
2. [[zero matrix]] $0_{m\times n}$ defines *zero transformation* $Z:R^n->r^m, Z(v)=0\in R^m$. 

##### Some non-matrix transformations
1. Define $S:R^2->R^2$ by $S(x,y)=(x+1,y+2)$. Its called a translation by (1,2). cannot be defined by a matrix since if it was a matrix transformation a 0 input would have to have an output of zero. 
2. Define $T:r^2->r^2$ by $T(x,y) = (x^2,xy)$ - not a matrix transformation. 