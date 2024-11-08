#comp250 
### Overview
Comparable [[interfaces|interface]] is used to define an ordering on objects of user-defined [[class]].
- Allows for sorting of objects within a given [[class]]
- Comparable comes from the java.lang [[package]] and contains the [[method]] `compareTo (Object)` of the [[generics|generic]] type
- The sort [[method]] from the Arrays package (default import) requires implementation of the comparable [[interfaces|interface]] to function.

### Implementation Guide
- Implement the compareTo method using the java documentation.
- + value if the object is greater then another
- 0 if the two objects are equal
- - value if the object is less then another
### Code
```java
public interface Comparable<T>{ // Generic type
	int compareTo (T o);
}
```