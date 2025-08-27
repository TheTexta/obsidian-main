#comp273 
##### Converting from binary to dec using 2's complement signed numbers
first digit is the sign (1=-; 0=+). invert everything if neg and **add 1**. 
##### Convert any base to another
take the original base and go to base 10. than divide by the new base and take the remainders in reverse order.
##### Largest number given x base
largest signed base32 number with n digits is (32^(n-1))-1

##### Converting decimal place in bin to dec
starts at 1/2 not 1/1

##### IEEE754 conversion
![[Screenshot 2025-03-06 at 1.20.15 PM.png]]
##### Converting with asciii
subtract 65 and count from there. 0=a, 1=b, etc. 

##### Simplifying boolean expressions
(A'+A)B = B
A+A'=1
AA=A
A+AB=A
AA'=0

##### Half Adder
A half adder circuit is a digital circuit that adds two single-bit binary numbers. It has two inputs, A and B, and two outputs, S (the sum) and C (the carry).

##### Full Adder
two half adders implemented with an OR gate. 

##### D Latch
A D latch is a basic memory element that captures and holds a single bit of data using a data input (D) and an enable signal. When the enable signal is active, the D latch transfers the input to the output, and when it is inactive, the output retains its previous state.


##### D Flip Flop
A D flip-flop is an edge-triggered memory element that captures the value of the D input on a specific clock edge (either rising or falling). Once triggered, it holds the captured value steady until the next clock event, ensuring synchronous data storage in digital circuits.
![[Screenshot 2025-03-08 at 2.33.51 PM.png]]
^ falling edge![[Screenshot 2025-03-08 at 2.34.19 PM.png]]
^ rising edge
![[Pasted image 20250308192308.png]]
##### RS Latch
An RS latch is a simple memory element made from cross-coupled logic gates (typically NOR or NAND) that uses two inputs—Set (S) and Reset (R)—to control a single stored bit. When the Set input is activated, the latch stores a high output, and when the Reset input is activated, it stores a low output; if both inputs are inactive, the latch retains its previous state.

##### MUX
Switches an input signal to one of several outputs through another signal 

##### Shift Register
A shift register is a digital circuit made up of a chain of flip-flops where the output of one flip-flop is connected to the input of the next, allowing data to be shifted along the chain one bit at a time, essentially moving data from one position to another by a single clock signal

##### PLA
![[Screenshot 2025-03-08 at 5.03.50 PM.png]]

### MIPS
##### SLT
Set on less than. If A<B? 1 else 0.

##### Register Names
By convention, registers have names to make it easier to code

\$16 -\$23 ➔ \$s0 -\$s7  (correspond to C variables)
\$8 -\$15 ➔ \$t0 -\$t7  (correspond to temporary variables)

##### Syntax
Operation Destination, Source1, Source2

##### addi
addi destination, source, number (+/-)

##### Register zero
MIPS defines register zero:\$0 or \$zero – It will always be 0![[Screenshot 2025-03-08 at 5.18.50 PM.png]]
can be used to negate a number (sub destination $0 input)
##### memory address
![[Screenshot 2025-03-08 at 6.04.33 PM.png]]

##### lw
load a word
lw DstReg, Offset(AddrReg)
- DstReg: register that will receive value
- Offset: numerical offset in bytes
- AddrReg: register containing pointer to memory

##### sw
store a word
sw DataReg, Offset(AddrReg)

##### beq
branch if equal
if the two registers are equal goto label
syntax: `beq $s1 $s2 label`

##### bne
branch if not equal
##### jal
jump and link
syntax: jal function_label
- jal saves the return address in register $ra.
- It then jumps to the specified function.

##### j
`j` jumps directly to a label without conditionals

##### IFELSE in Mips
![[Pasted image 20250309220206.png]]

##### do-while loops in mips
![[Screenshot 2025-03-09 at 10.04.24 PM.png]]

##### Inequalities in MIPS
![[Screenshot 2025-03-10 at 11.35.18 AM.png]]

geq achieved by inverting less than.
```asm6502
slt $t0,$s0,$s1     # $t0 = 1 if $s0 < $s1 (g < h)
beq $t0,$0, Geq     # if $t0 == 0, goto Geq ( g >= h )
```


##### slti
sltiis the immediate version ofslt

##### functions in mips
Parent/Caller should save the arguments in $a0, $a1, $a2, $a3
Child/Callee should save the return values in $v0, $v1

##### return address
Register for the return address  $ra
Parent/Caller saves the returning address in $ra before jumping
Child/Callee jumps to the $ra after done![[Screenshot 2025-03-10 at 11.56.48 AM.png]]

##### the stack

```
# move the stack pointer down
addi $sp, $sp,-4.    # store the content of $s0 into address $sp
sw $s0, 0($sp)
```

If you are a subroutine that will call another subroutine, follow this convention–Before you call anyone, push the return address in **$ra** on the stack–When you are done calling, pop the return address (that you will need to return to your caller) off the stack into $ra
* Also follow conventions for save and temporary registers!
	* Save registers, $s0 through $s7 must be left as you found them!
	* 
##### Register conventions
![[Screenshot 2025-03-10 at 1.15.00 PM.png]]
