#comp273 
IEEE 754 used in nearly all computers today

defines two representations
- single precision (float 32bit)
- double precision (double 64bit)

Single precision
divides a single 32 bit word into 3 fields
![[Screenshot 2025-01-15 at 12.08.08 PM.png]]
does not use 2's complement - bias is always 127

numbers are in normalised form always

$-0.75_{10}$ to floating point
$S=1$ (sign negative)
$0.75*2=1.5$
$0.5*2=1$
$-0.11_2 \times 2^{-1}$
$E-127=-1$
$E = 126_{10} = 0111 1110_2$


Special cases:
nonzero divided by zero - results in +/- infinity
0/0 = NaN
![[Screenshot 2025-01-15 at 12.21.19 PM.png]]

floating point addition
1. align the decimal points
2. add the significands
3. normalize
4. round
5. compute the sign
6. 