#math222 
let $x_0$ be a fixed number. we call [[power series]] around $x_0$ (on centred at $x_0$) a series of the form $$\sum_{m=0}^{\infty}{c_m(x-x_0)^m}=c_0+c_1(x-x_0)+c_2(x-x_0)^2+...$$
where $x$ is the [[variable]] and $x_m$ are constants called the [[coefficients|coefficients]]. 

### Do functions converge? (dependent on [[coefficients]])
at $x=x_0$, it is obvious that the series converges. sum $=$ $c_0$ (clearly bruh lmfao)

you should know:
1. [[geometric series]] (it is a [[power series]])
	- which converges $\iff |x-x_0|<1$
	- if converges absolutely for all $x$ such that $|x-x_0|<1$
2. $\sum_{m=0}^{\infty}{\frac{(x-x_0)^m}{m!}}$ (the [[exponential power series]])
	- apply the [[ratio series test|ratio test]] with $a_m = \frac{(x-x_0)^m}{m!}$
	- $\lim_{m \to \infty} \left|\frac{a_{m+1}}{a_m}\right| = \lim_{m \to \infty} \frac{|x-x_0|}{m+1} = 0$
	- since $L=0 < 1$, the [[series]] converges absolutely for all $x$ (radius of convergence $R = \infty$)
	- recall [[ratio series test|ratio test]] cases: $L<1$ $\Rightarrow$ convergent, $L>1$ $\Rightarrow$ divergent, $L=1$ $\Rightarrow$ inconclusive
3. $\sum_{m=0}^{\infty}{m!(x-x_0)^m}$
	* apply the [[ratio series test|ratio test]] with $a_m = m!(x-x_0)^m$
	* $\left|\frac{a_{m+1}}{a_m}\right| = (m+1)|x-x_0|$
	* as $m \to \infty$, $(m+1)|x-x_0| \to \infty$ if $|x-x_0|>0$
	* therefore:
		* if $x=x_0$, the [[series]] converges (only the $m=0$ term survives)
		* if $x \neq x_0$, the [[series]] diverges (radius of convergence $R=0$)

## Theorem: [[Convergence of Power Series Theorem]]