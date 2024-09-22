#comp250 
If a [[variable]] is final it can never be changed. Compile time error will occur if you try. Final types can be misleading when assigning [[reference type]] variables since the values stored with the reference can still be changed without changing the [[variable]]. 

```java
final int x=3;
x=10 // compile-time error
```
