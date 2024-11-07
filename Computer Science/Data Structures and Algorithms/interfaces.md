#comp250 
interfaces can be public or private. can list and declare methods and fields. 
by default:
- methods public and abstract
- fields public static and final

- interfaces cannot implement methods unlike [[abstract]] classes.
- interfaces describe behaviours
- 

### Declaration
```java
public interface MyInterface { // implicitly absract
	public int spook(); // implicitly abstrat
	public void runAway(); // only have to declare signatures.
}
```


classes can use interfaces through implementing them. java interfaces can be extended by other interfaces. 

### Instantiation
you can instantiate classes which implement interfaces to the interface type
```java
public interface Monster { ... }
public interface Green { ... }
public class Orc implements Monster, Green { ... }

Monster myOrc = new Orc();
```