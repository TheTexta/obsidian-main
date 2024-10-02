#comp250 
Integer, Double, and Character wrap a value of the [[primitive type|primitive type]] int, double and [[char]] in an [[object]]. turning [[primitive type|primitive types]] into [[immutable types|immutable]] [[Reference Type|reference types]]. Because they are [[immutable types|immutable]] like [[string|strings]] every time you update the [[object]] a new [[object]] is created. Useful because we can get code that can be generalised

the conversion between the primitive types and their wrappers is done automatically (an example of [[autoboxing]])
```java
Integer x = 5; // Does NOT cause a compile time error
```
