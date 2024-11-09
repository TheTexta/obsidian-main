#comp250 
### Overview
[[for each loops]] can only be used when the collection is [[Iterable]].  

An [[Iterable]] is an [[object]] which can be iterated and the [[iterator]] is the tools which allows for the object to be iterated.

Generally the class used to implement the iterator interface is nested within the class implementing the iterable interface - [[Iterator]] SSLIterator is nested within the [[Iterable]] [[Linked list|SLinkedList]] [[class]].
![[Explaning the implementation of iterables and iterators.png]]
### Implementation
- Generally you write classes that implement the iterable interface which includes [[iterator]] class defined inside the [[Iterable]] outer shell.
- Because the [[Iterable]] interface implements a [[method]] returning the type [[Iterable]] we need create a class which can create such an object. 
##### Example Implementation
```java
public class MyCollection<T> implements Iterable<T> {
	public MyIterator<T> iterator(){
		return new MyIterator<T>(this);
	}
}
public class MyIterator<E> implements Iterator <E> {
	public MyIterator(MyCollection<E> c){
	...
	}
}
```
### Code
```java
public interface Iterable<T>{
	public Iterator<T> iterator();
}
```

#comp250 
### Overview
[[for each loops]] can only be used when the collection is [[Iterable 1]]. 

### Implementation