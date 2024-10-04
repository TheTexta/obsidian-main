#math133 
Let $A=\pmatrix{a&b\\c&d}$. Define the determinant of $A$ by:
$$det(A)=ad-cd$$
If $det(A)\neq 0$ then $A$ invertible and $$A^{-1}=\frac{1}{det(A)}\pmatrix{d&-b\\-c&a}$$
##### Proof
verify
$$AA^{-1}=\pmatrix{a&b\\c&d}(\frac{1}{det(A)}\pmatrix{d&-b\\-c&a})$$
$$AA^{-1}=\frac{1}{det(A)}\pmatrix{a&b\\c&d}\pmatrix{d&-b\\-c&a}$$
$$AA^{-1}=\frac{1}{det(A)}\pmatrix{ad-cb&-ab+ba\\cd-dc&-cb+ad}$$
$$AA^{-1}=\frac{1}{ad-cd}\pmatrix{ad-cb&0\\0&-cb+ad}$$
$$AA^{-1}=\pmatrix{1&0\\0&1}$$
$$AA^{-1}=I$$
