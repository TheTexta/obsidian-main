#math133 
Let $A,B$ $n\times n$ then,
$det(AB)=det(A)\cdot det(B)$


**Case 1**: $A$ is [[Invertibles|invertible]], then
$A=F_1,F_2,...,F_k$ where $F_i$ [[elementary matrices|elementary]]
then
$det(AB)=det(F_1F_2...F_k\cdot B)$
$=det(F_1)\cdot det(F_2...F_k\cdot B)$
$=det(F_1)\cdot det(F_2) \cdot ... \cdot det(F_k) \cdot det(B)$
$=\det(F_1F_2)\cdot ... \cdot det(F_k) \cdot det(B)$
^ using lemma 22(2)
$= \det (A) \cdot \det(B)$

**Case 2:** $A$ is not invertible, then
$det(A)=0$
then $AB$ must not be [[Invertibles|invertible]], since if $(AB)^{-1}$ exists,
(AB)(AB)^{-1}=I
A(B(AB)^{-1})=I
then A^{-1}, but A not invertible
then $det (AB) = 0$, both sides of formaula are O. []

[[Corollary 25]]