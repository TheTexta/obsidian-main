#comp250 
- Base clause:
	- Which one/more basic/initial element of the set
- 1+ Inductive clause:
	- Rules on how to generate new elements of the set from the old ones. 
- Final clause:
	- States that no other element is part of the set
##### Example - Natural Numbers
*Base Clause:*
0 is a natural number

*Inductive Clause:*
If n is a natural number then n+1 is also a natural number

*Final Clause:*
Nothing else is a natural number.

### mathematical induction
consider a statement of the form:
- for all $n\geq n_0, P(n)$ is true
where $n_0$ is some constant and proposition $P(n)$ has value true or false for each $n$.

#### (weak) mathematical induction
To prove a property by mathematical induction, we proceed as follows:
- base case: show that the property holds for the basic/initial elements of the set.
- Induction step: assume the property hold for some element $n$ (induction hypothesis). Show that the property also holds for any element generated from n using the inductive clauses.
- Conclusion: The property holds for all elements

##### Example
- for all $n\geq n_0, P(n)$ is true

for all $n \geq 1$,
$$1+2+3+...+(n-1)+n=\frac{n(n+1)}{2}$$
This is a property of natural numbers.

We need to prove the following:
- base case: $P(n_0)$ is true, i.e. the property holds for $n_0$ which in this case is $1$
- induction step: assume $P(k)$ is true, ie. the property holds for an element $k$. Prove that $P(k+1)$ is true, ie. the property holds for $k+1$.

$$\forall n \geq 1,1+2+...+n=\sum_{i=1}^n{i}=\frac{n(n+1)}{2}$$
Base Case: Let $n=1$ - $1=\frac{1\cdot 2}{2}=1$ therefor true
Ind. Step: IH (Inductive Hypothesis):$\sum_{i=1}^k{i}=\frac{k(k+1)}{2}$ To prove $\sum_{i=1}^{k+1}{i}=\frac{(k+1)(k+2)}{2}$![[Screenshot 2024-11-09 at 4.41.19 PM.png]]
This statement holds true for all natural numbers. 
##### Example 2
![[Screenshot 2024-11-09 at 4.55.56 PM.png]]
#### (Strong) Mathematical Induction
- sometimes one would like to assume the induction hypothesis not only for the previous element, but also for smaller elements. this leads to a logically equivalent proof method called strong (or complete) mathematical induction.
- To prove a property by strong mathematical induction:
	- Induction step: Assume the property hold for all elements less than an arbitrary k. (induction hypothesis) show that the property also holds for the k element which was generated using the inductive clauses.
	- Conclusion: The property holds for all elements.
##### Fibonacci numbers are proved by strong mathematical induction
- $1,1,2,3,5,8,13,21,34,55,89,144,...$
- let $f_n$ denote the nth Fibonacci number. How can we define the sequence above?
- Base clause: f_0 = f_1 = 1 are Fibonacci numbers
- Inductive Clause: If $f_{n-1}$ and $f_{n-2}$ are Fibonacci numbers, then $f_n=f_{n-1}+f_{n-2}$ is a Fibonacci number

