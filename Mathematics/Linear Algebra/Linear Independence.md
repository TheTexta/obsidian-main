#math133 
In R^2 with only e_1 and e_2 each vector has unique representaiton in form ae_1 and be_2. each vector has inf many represenations. 

Suppose U=span{vectors u_1 to u_m} and v\in U and v

Let X={u_1,u_2,...,u_m} vectors in \mathbb{R}^n. X called linearly independent if the only solution to the following
$$\vec{0}=c_1u_1+...+c_mu_m$$
is the trivial solution c=0 for all.

X is called linearly dependent if not linearly independent. That is, there exists cs where some are not zero such that you can get the zero vector from them anyway.
$$\vec{0}=c_1u_1+...+c_mu_m$$
Note: empty set is considered linearly independent. 

If $X=\{u_1,...,u_m\}$ linearly independent, then every $v\in$ span X can be expressed uniquely in the form
$$v=c_1u_1+...+c_mu_m$$

To show independence solve the given vectors as a linear system. If the solution is trivial the solution is independent. Elsewise it is dependent. 

Vectors are dependent if and only if they can be written as a linear combination of other vectors
##### Lil example of dependence
![[Screenshot 2024-11-27 at 8.14.42 AM.png]]

##### Set of one vector
a set of the single vector v is dependent if and only if v=0. 
$$\text{A set containing a single vector } \{\vec{v}\} \text{ is linearly dependent} \iff ( \vec{v} = \vec{0} ).$$
##### set of two vectors
$\{u,v\}$ dependent $\iff$ $u=cv$ or $v=cu$. where one is some multiple of the other

##### set of any vectors containing the zero vector is dependent
since $\vec{0}=1\cdot \vec{0}$ is a dep. relation.


### Problem
let $x,y\in \mathbb{R}^n$
1. show $span\{x,y\} = span\{x+y,x-y\}$
2. if $x,y$ lin independent, show $x+y, x-y$ also independent

Sol
1. show every $v$ $\in$ span{x,y} is also in span {x+y,x-y}
2. 