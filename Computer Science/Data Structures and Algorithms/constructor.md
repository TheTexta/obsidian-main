#comp250 
[[object|Objects]] have constructor [[method|methods]] which are run on creation of an instance of an object. You can have multiple constructors because of overloading. 

- The name of a constructor must be the same as the name of the class
- It has no return type
- It is non-static (meaning an instance is required for the method to be ran)


When you don't write a constructor the default is below (it does FUCK ALL)
```java
public ClassName(){

}
```


- always use `this.variableName` when assigning local [[variable|variables]] to attributes of objects