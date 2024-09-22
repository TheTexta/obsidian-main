#math133 
##### Def
Given $S:R^n->R^m$, $T:R^m->R^p$ transformations, define the *composition* $T\cdotS:R^n->R^p$ by, for each $v\in R^n$,

$(T\cdot S)(\vec{v})=T(S(\vec{v}))$
![[Screenshot 2024-09-22 at 3.44.28 AM.png]]

##### Example
A=((1,2)(0,-3)), B=((2,1),(1,-1))
Find formulas for T_A \cdot T_B:R^2->r^2 and T_B \cdot T_A:R^2->r^2

So
$(T_a \cdot T_b)(x,y)=T_A(T_B(x,y))=T_A((2,1),(1,-1))(x,y)=T_A(2x+y,x-y)$
$=((1,2)(0,-3))(2x+y,x-y)=(2x+y+2x-2y,0-3x+3y)=(4x-y,-3x+3y)$

If we set $c=((4,-1),(-3,3))$ then $T_c(x,y)=(4x-y,-3x+3y)$.

we will define the product A B by A B=C