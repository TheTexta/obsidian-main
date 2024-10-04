#comp250 
### Overview
- made-up of nodes which attach to other nodes and contain a single reference to a variable. nodes are not necessarily stored next to each other. 
- ![[linked list vs array list.png]]
- addFirst (e)
- removeFirst ()
- addLast (e)
- removeLast()
- More efficient then [[ArrayList|arraylists]] when adding / subtracting elements (O(N) vs O(1))
- doubly linked lists include pointers to previous and future nodes
- singly only include pointers to future nodes
- more shape complex then arraylists (2x-3x)

### Implementation of Singly Linked List Node
```java
class SNode {
	Shape element;
	SNode next;
}

SNode myNode = new SNode();
myNode.element = new Shape("Triangle");
```

Usually only keep pointers to the first and last node in a singly linked list. We dont care about keeping pointers to the in between nodes since we can find them using the beginning and the end nodee.

```java
public class SLinkedList {
	private SNode head;
	private SNode tail;
	private int size; // Reduces runtime for list size to instant.

	private class SNode {
		Shape element;
		SNode next;
		
	}
}

SLinkedList list = new SLinkedList();
```