#comp250

Allows you to iterate through [[object|objects]] that represent a collection. The tools which allow you to go through a collection (like a [[linked list]]). NOT THE SAME AS [[Iterable]].  

An [[Iterable]] is an [[object]] which can be iterated and the [[iterator]] is the tools which allows for the object to be iterated.

### Code
```java
public interface Iterator<T> {
	boolean hasNext(); // self explanetory
	T next(); // returns current and advances to next
	void remove(); // optional ignore it
}
```