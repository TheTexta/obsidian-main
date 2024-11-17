#comp250 
A rooted tree where each node has at most 2 children which are differentiated by left and right side.

```java
class BTree<T>{
	BTNode<T> root; 
	class BTNode<T>{   
		T element;
		BTNode<T> leftchild;
		BTNode<T> rightchild;
	} 
}
```

### Traversal
![[Screenshot 2024-11-17 at 3.15.07 PM.png]]
