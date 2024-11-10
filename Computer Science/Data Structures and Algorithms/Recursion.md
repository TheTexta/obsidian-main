#comp250 
### Overview
Recursive methods consist of the following:
- Base Case: one (or an inf. number) of terminating scenario that does not use recursion to produce an answer.
- Recursive or [[Induction|inductive]] step(s): rules that determine how to produce an answer from simpler cases
- Its best to think about the base case and recursive steps when implementing a recursion algorithms rather than observing every subroutine trust it will function correctly. 
- *recursive steps* - rules that determine how to produce an answer from simpler cases
- *base case* -  one or finite number of scenarios that do not use recursion to produce a result
- knowing that the method has to work on a simplified version of the task ($n-1$ version) given helps understanding how to create an effective algorithm.

### Algorithms using recursion
##### Factorial
*Definition*
**Base Case**: $0!=1$
**Recursive Step**: $n!=n*(n-1)!$

*Code* - either def works and any iterative def can be expressed recursively and vise-versa.
```java
// Iterative Def (often more effecient but less elegant)
public static int factorial (int n){
	int result = 1;
	for (int i=2,i<=n,i++){
		result = result * i;
	}
	return result;
}

// Recursive Def (often less efficient but more elegant)
public static int factorial (int n){
	if (n==0){
	return 1
	}
	return n * factorial(n-1);
}
```

##### Fibonacci
```java
public static int fibonacci (int n){
if (n==1||n==0)
}
```
![[Screenshot 2024-11-09 at 5.27.14 PM.png]]
We keep on computing the fibonacci number for 244 - very inefficient

##### Reversing a List
Take min element to front and sort list
##### Tower of Hanoi
```java
tower(n, start, finish, other) { // e.g. tower(5,A,B,C)
	if(n==1) {
		move from start to finish. 
	} else {
		tower(n-1, start, other, finish)
		tower(1, start, finish, other)
		tower(n-1, other, finish, start)
	}
}
```

##### [[Binary Search]]
##### [[Merge Sort]]