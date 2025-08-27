#math222 
**Theorem (Convergence of [[Power Series]]):**  
For a [[power series]] $\sum_{m=0}^{\infty} c_m (x - x_0)^m$, there are only three possibilities:

1. The series converges only at the center $x = x_0$ (radius of convergence $R=0$).  

2. The series converges absolutely for all $x \in \mathbb{R}$ (radius of convergence $R=\infty$).  

3. There exists a finite radius $R > 0$ such that:  
   - the series converges absolutely for all $x$ with $|x - x_0| < R$,  
   - the series diverges for all $x$ with $|x - x_0| > R$,  
   - at the boundary $|x - x_0| = R$, convergence may or may not occur (must be checked separately).


**Remark:**  
- At the boundary points $x = x_0 \pm R$, the series $\sum c_m (x - x_0)^m$ may **either converge or diverge**; this must always be tested individually.  
- $R$ is called the **radius of convergence**.  
  - In Case 1: $R=0$.  
  - In Case 2: $R=\infty$.  
- The set of all $x$ for which the series converges is called the **interval of convergence**.