#math133 
theorem 7: Let $A$ be and $m\times n$ matrix $\vec{x}=\pmatrix{x_1\\...\\x_n}$ a [[vector]] of variables, consider [[homogeneous system]].  $A\vec{x}=\vec{0}$. If $\vec{v}_1,\vec{v}_2,...,\vec{v}_l\in\mathbb{R}$ are all solutions to the system (ie. $A\vec{v}_i=\vec{0}$) and $c_1,c_2,...,c_l\in\mathbb{R}$ scalars. The linear combination $c_1v_1 + c_2v_2+...+c_lv_l\in\mathbb{R}$ is also a solutions to $A\vec{x}=\vec{0}$.
- Proof: verify by substitute w into $A\vec{x}=\vec{0}$ make sure equal:
			$A\vec{w}=A(c_1v_1+...+c_lv_l)$
				$= A(c_1v_1) + ... + A(c_lv_l)$
				$= c_1Av_1+...+c_lAv_l$
				$=c_1(\vec{0})+...+c_l(\vec{0})$
				$=\vec{0}+...+\vec{0}$
				$=\vec{0}$
				i.e. Equations $A\vec{x}=\vec{0}$ holds so $\vec{w}$ is a solution
	*this only works because the solution is [[homogeneous system|homogenous]]* ($\vec{0}$ as opposed to a solution of $\vec{b}$)
	