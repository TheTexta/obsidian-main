#comp250 
- [[Class|Classes]] can be derived from other [[Class|classes]]
- a [[class]] derived from another is a [[subclass]]
- the class from which the [[subclass]] is derived is called the [[superclass]]
- all classes have the [[Object class]] [[superclass]]

```java
public class Animal {
	String name;
	public Animal(String name){
		this.name = name;
	}
}

public class Dog extends Animal{
	public void bark(){
		System.out.println("SKKIBIIIDI");
	}
}
```