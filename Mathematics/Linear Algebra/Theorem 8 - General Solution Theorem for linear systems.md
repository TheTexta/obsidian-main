#math133 
Let $A\vec{x}=\vec{b}$ be linear system and suppose $\vec{p}$ is a solution (i.e. $p$ substituted in for $x$ will give $\vec{b}$ - $Ap=\vec{b}$) called "particular solution". Then
1. every vector of the following form $\vec{p}+\vec{v}$ where $\vec{v}$ is a solution to the homogenous system Ax=0 (same [[coefficient matrix]])  (ie. $A\vec{v}=\vec{0}$) is also a solution to $Ax=b$. 
2. Every solution to $A\vec{x}=\vec{b}$ has the form $\vec{p}+\vec{v}$ where $\vec{v}$ solution to $A\vec{x}=\vec{0}$. 
- Illustration
	$A=\pmatrix{1&2&0&-3\\0&0&1&4}, \vec{b}=\pmatrix{1\\5}$
	solve:
		$x_1=1-2s+3t$
		$x_2=s$
		$x_3=5-4t$
		$x_4=t$
	ie.
		$\vec{x}=\pmatrix{-1-2s+3t\\s\\5-4t\\t}=\pmatrix{-1\\0\\5\\0}+s\pmatrix{-2\\1\\0\\0}+t\pmatrix{3\\0\\-4\\1}$
		set $s=0,t=0$ ($s$ and $t$ represent $\vec{v}$ from the theorem) get a solution $\vec{x}=\vec{p}=\pmatrix{-1\\0\\5\\0}$ ie. $A\vec{p}=\vec{b}$
		For each $s,t$ $\vec{v}$ is sol to $A\vec{x}=\vec{0}$
		$Av=A(p+v-p)$
		  $=A(p+v)-Ap$ 
		  $=b-b$
		  $=\vec{0}$

##### Proof
1. Assume Av=0, Ap=b then $p + v$ is sol to $Ax=b$ since
		$A(p+v)=Ap+Av$
			   $= b + \vec{0}$
			   $= b$
2. Let $Au=b$, ie $u$ is a sol to $Ax=b$. Set $v=u-p$, making $u=p+u-p = p+v$
	 Then $v$ is a sol to $Ax=0$ since $Av=A(u-p)=b-b=0$