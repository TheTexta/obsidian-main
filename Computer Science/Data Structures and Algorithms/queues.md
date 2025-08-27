#comp250 
A queue is a structure ([[abstract]] data type) where you take elements from the front and load them to the back (dequeue and queue respectfully)


|                        | enqueue(e)          | dequeue       |
| ---------------------- | ------------------- | ------------- |
| singly [[linked list]] | addLast(e)          | removeFirst() |
| doubly [[linked list]] | same or addFirst(e) | removeLast()  |
| [[arraylist]]          | addLast(e)          | removeFirst() |

##### Implementing a queue with a circular array
- tail = (head + size - 1) [[modulo|mod]] length
- if tail when updated = head then we resize
- when resizing you have to be careful. put the head at zero and the tail closer to the end.
- 