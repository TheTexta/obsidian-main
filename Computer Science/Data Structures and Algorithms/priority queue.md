#comp250 
Like [[queues]] but with a more general definition of which element to remove next, the one with highest priority - like a hospital emergency room.

The queue can dynamically update the order of the elements depending on its priority - rather than first come first served. You can also just use [[heaps]]. Heaps are the best way to implement priority queues. But sorted lists, binary search tree and balanced binary search trees can be used.

```java
add(key)
removeMin()
```

