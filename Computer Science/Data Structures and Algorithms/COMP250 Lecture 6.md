#comp250 
- when using println() with objects it calls the method toString() on the object to display the results
- you can write a [[toString method]] method in any class
- mutable vs immutable
	- immutable
		- if when you create a class you make all the fields private and you do not write any mutator methods then you effectively created an immutable type
		- if the only way to assign values to fields is through the constructor then the values of the Object cannot be changed after it has been created. 
	- mutable
		- 