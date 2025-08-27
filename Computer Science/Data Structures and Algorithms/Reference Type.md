#comp250 
In java reference types (eg Strings, Arrays - always [[UpperCamelCase]] [[variables]]) are [[object|objects]] and the variable which you define through a reference type merely stores the reference to the location in memory containing the data. Reference type variables store values that point to memory locations, they are pointers.

because of this behaviour reference type objects can be assigned the same reference point for multiple variables. Any reference type variable can have a [[null]] value - indicating the absence of an address. 

eg. demonstration of array [[mutability]]
```java
int[] a = {1,2,3};
int[] b = a;
a[0]=4;

System.out.println(a[0] + " " + b[0]) -> "4 4"
```

