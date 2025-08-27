#comp250 
### Overview
Comparable [[interfaces|interface]] is used to define an ordering on objects of user-defined [[class]].
- Allows for sorting of objects within a given [[class]]
- Comparable comes from the java.lang [[package]] and contains the [[method]] `compareTo (Object)` of the [[generics|generic]] type
- The sort [[method]] from the Arrays package (default import) requires implementation of the comparable [[interfaces|interface]] to function.
- `Character`, `Integer`, `Float`, `Double`, `BigInteger`, etc. all implement `Comparable<T>`
- Use `compareTo()` over `<` for these kind of classes

### Implementation Guide
- Implement the compareTo method using the java documentation.
- + value if the object is greater then another
- 0 if the two objects are equal
- - value if the object is less then another
- When using the method ensure the relation ship is anti [[commutative]] and [[transitive]] e.g. `(t1.compareTo(t2)==0)==t1.equals(t2))`
- You can use compareTo() to compare multiple characteristics of a [[class]] at once assuming they implement the [[interfaces|interface]]. eg. comparing orcs you can compare there heights and weapons by calling `compareTo` to the weapon assuming the weapon [[object]] implements the `compareTo()` method separately.
### Code
```java
public interface Comparable<T>{ // Generic type
	int compareTo (T o);
}
```