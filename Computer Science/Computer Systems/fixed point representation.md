#comp273 
$$a_n a_{n-1} \dots a_1 a_0 . a_{-1} a_{-2} \dots a_{-m}$$
- choose n and m
- radix point is always in the same position
- easy implementation
- limited range
	- using with n=3 and m=3, its not possible to store 0.0002
- allows for binary to fractions
	- $0.11001_2 = 11001_2 \times 2^{-5}=\frac{25}{32}$
	- 0.