#comp250 
A class contains [[method]]s and names are written in [[UpperCamelCase]]. The class name must match the name of the file. each time we define a class we create a new [[object]] type with the same name. A class is a blueprint for a type of [[object]]. 

className.java would look like
```java
public class className {
// some data declared here - fields / attributes
<modifier> <type> <variable_name>
public className(){
	// constructor
}
// declare other methods

}
```

#### Using a class outside of its package
1. specify entire path of class
```java
animals.Dog() myDog = new animals.Dog();
```
2. import the package member
```java
import animals.Dog;
```
3. import the entire package (dont use unless you need multiple things cause thats BAD practice)
```java
import animals.*;
```
