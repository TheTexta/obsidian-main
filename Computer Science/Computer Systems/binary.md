#comp273 
How to represent sign and magnitude
- Use the most sig bit to rep sign
	- +13 = 0000 1101
	- - 13 = 1000 1101
	- Problems
		- two representations for zero 0000 0000 and 1000 0000
		- cannot easily add numbers
- invert each bit
	- +13 = 0000 1101
	- -13 = 1111 0010
	- problems
		- still two zero representations
		- answer off by 1
		- incorrect overflow
- twos complement - invert bits and add one
	- most significant bit (MSB)
		- 1 if neg
		- 0 if pos
		- msb rep sign
	- n-bit negative numbers are defined as negative (N) $2^n-N$
	- unique zero!
	- range from $-2^{n-1}$ to $+2^{n-1} -1$
	- one extra negative number than positive
	- overflow happens when the two numbers are not opposing signs (positive and negative)
- [[packed decimal]]
- [[parity]]
![[Screenshot 2025-01-15 at 10.39.42 AM.png]]
