#comp250 
when we cast type to another nonexplicitly

```java
Animal myDog = new Dog();
```

You have to [[explicitly downcast]] to use methods in the Dog class exclusively
```java
Dog myDog2 = (Dog)myDog;
```
