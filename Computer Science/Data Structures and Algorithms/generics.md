#comp250 

### Example
```java
public class Cage<T>{
	private T occupant;

	public void lock (T p){
		this.occupant = p;
	}
	
	public T peek(){
		return this.occupant;
	}
	
	public void release(){
		this.occupant = null;
	}
}

Cage<Dog> crate = new Cage<Dog>(); // now in the crate we can lock only Dogs.
```
### Bounded type
- we can restrict classes with the extends keyword (inheriting [[Class|classes]] or [[interfaces]])
```java
public class Cage<T extends MonsterLike> { ... } // will only allow for MonsterLike classes to be used.
```
### Naming Conventions
- E - Element
- K - Key (used in map)
- N - Number
- T - Type
- V - Value
