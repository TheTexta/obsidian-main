#math133 
$l_1(t)=p_1+td_1, l_2(t)=p_2+td_2$
1. parallel if $d_1=cd_2$ for some $c\neq 0$
2. Intersecting if $l_1(t_1)=l_2(t_2)$
3. skew lines otherwise

### examples
Prob
$$\begin{align*} \ell_1 : & \begin{cases} x = 4 + 3t \\ y = 1 + t \\ z = -3 - t \end{cases} \\[10pt] \ell_2 : & \begin{cases} x = -1 + 2t \\ y = -1 + t \\ z = -3 + t \end{cases} \end{align*}$$
are they parallel, int or skew?
$$\begin{align*}
\vec{d}_1 &= \begin{pmatrix} 3 \\ 1 \\ -1 \end{pmatrix}, \quad \vec{d}_2 = \begin{pmatrix} 2 \\ 1 \\ 1 \end{pmatrix}
\end{align*}
$$
vectors not parallel, lines not parallel.
Int? use dif param names for $t$ - $s$ in $l_2$ (unless t is time).
$4+3t=-1+2s$
$1+t=-1+s$
$-3-t=-3+s$

linear system - solve like how we alr know to! sol for $t=-1$ and $s=1$