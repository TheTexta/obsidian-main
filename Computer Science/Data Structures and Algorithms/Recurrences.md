#comp250 
A recurrence is an equation or inequality that describes a function in terms of its value on smaller inputs.

e.g. Fibonacci $F(n)=F(n-1)+F(n-2)$


##### Example 1 - Reversing a List
$T(1)=b$, $T(n)=c+T(n-1)$, 
$T(n-1)=c+c+T(n-2)$
$T(n)=kc+T(n-k)$ substitute $k$ with a value such that $T(n-k) = T(1)$ ie. $(n-1)$
$T(n)=(n-1)c+T(1)$
$T(n)=(n-1)c+b=cn+b-c=\Theta (n)$

Runs in $\Theta (n)$
##### Example 2 - Sorting a list
$T(1)=a$
$T(n)=cn+T(n-1)+b$
$T(n)=cn+T(n-1)$
$T(n)=kn+T(n-k)$
$T(n)=(n-1)n+T(1)$
$T(n)=(n-1)n+a$
$T(n)=(n-1)n$
$T(n)=n^2-n$

Runs in $\Theta (n^2)$

##### Example 4 - Binary Search
*Worst Case*
$T(1)=b$, $T(n)=c+T(\frac{n}{2})$
$T(\frac{n}{2})=c+T(\frac{n}{4})$
$T(n)=c+(c+T(\frac{n}{4}))$
$T(n)=kc+T(\frac{n}{2^k})$

$2^k=n$
$k\cdot log(2)=log(n)$
$k=log_2(n)$

$T(n)=log_2(n)+T(1)$
$T(n)=log_2(n)+b$
$\Theta (log(n))$
