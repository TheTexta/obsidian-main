#math133 

![[polynomial interpretation.png]]
can find polynomial $f(x)$ such that $f(x_i)=y_i$ for all $i$. this can be done with polynomial of degree $n$ where $n=i-1$. 
$$\begin{pmatrix} 1 & x_0 & x_0^2 & \dots & x_0^n \\ 1 & x_1 & x_1^2 & \dots & x_1^n \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 1 & x_n & x_n^2 & \dots & x_n^n \\ \end{pmatrix} \begin{pmatrix} a_0 \\ a_1 \\ a_2 \\ \vdots \\ a_n \\ \end{pmatrix} = \begin{pmatrix} y_0 \\ y_1 \\ \vdots \\ y_n \\ \end{pmatrix}$$
Sys of $n+1$ equations is $n+1$ variables
$$V=\begin{pmatrix} 1 & x_0 & x_0^2 & \dots & x_0^n \\ 1 & x_1 & x_1^2 & \dots & x_1^n \\ \vdots & \vdots & \vdots & \ddots & \vdots \\ 1 & x_n & x_n^2 & \dots & x_n^n \\ \end{pmatrix}$$
This is a [[vandermonde matrix]]
$det(V)=\text{produce of all factors of form } (x_i-x_j) \text{ where } i>j$
$det(V)=(x_2 - x_1)(x_3 - x_1)(x_3 - x_2) \dots$
$= \prod_{\substack{n \geq i > j \geq 1}} (x_i - x_j)$
we have all $x_i$ distinct, hence $det(V)\neq 0$. hence $V$ [[invertibles|invertible]] so [[linear systems|system]] has unique solution