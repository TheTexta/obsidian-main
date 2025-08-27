#comp250 
A complete [[binary tree]]. Meaning all levels less then height $h$ are full, with nodes at level $h$ as far to the left as possible. 

##### Min heap
Each elements key is less than its children's element key.

##### Removemin
swap the bottom right element with the top element (upHeap) - deleting the bottom right element in the process. Perform downHeap thereafter. 

##### downheap
take the smaller element of the two children and swap continuously. 


##### Heap array implementation
![[Screenshot 2024-11-25 at 12.56.51 PM.png]]
parent = child/2
left = 2\*parent
right = 2\*parent +1


##### building a heap (fast)
observe: half of nodes are leafs. The last