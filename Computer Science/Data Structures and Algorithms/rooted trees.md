#comp250 
### Overview
A tree is a collection of nodes/vertexes
##### Edges
- a directed edge is ordered pari of nodes ($v_i,v_j$) (from, to)
- an undirected edge (for unrooted trees)
- number of edges where $n$ is nodes = $n-1$

for some trees
- edges are directed from parent to child
- edges are directed from child to parent
- edges are directed from child to parent and from parent to child
- edge direction is ignored. e..g common with non-rooted trees
##### Nodes
- a child is a node directly connected to another node when moving away from the root.
- a parent node is directly connected to another node when moving towards the root. 
Every node except the root is a child and has exactly one parent

- an internal node is one with $\geq 1$ child
- a leaf/external node is one with zero children

path
- ancestor node is the node at the beginning of a path
- descendent node is the one at the end of the path
##### Paths
- a path is a sequence of nodes (v_1,v_2,...,v_k) such that ($v_i,v_{i+1}$) is an edge
- the length of a path is the number of edges in the path (number of nodes in path - 1)
##### Recursive definition of a tree
- if n>0 then one of the nodes is the root $r$
- if n>1 then n-1 non-root nodes are partitioned into subsets $T_1,T_2,...,T_k$, each of which is a tree (subtree), and the roots of the subtrees are the child of root $r$.

Another def
- tree=root|(root listOfSubTrees)
- listOfSubTrees=tree|tree listOfSubTrees
*listOfSubTrees cannot be empty*
##### Depth
the depth of a node is the length of the path from the root to the node. you can compute the depth on the spot (expensive), we can use a parent link (annoying), we can use a variable in the node to keep track when children are created (i like this one).

##### Height
the height of a node is the *maximum* length of a path from that node to a leaf. can compute recursively by taking the maximum of a subnode and adding one. 

### Implementation
create a data type to represent tree nodes. represent a tree with a point to the root node.
```java
class TreeNode<T>{
	T element;
	ArrayList<TreeNode<T>> children;
	TreeNode<T> parent; // optional
}
```

another implementation
```java
class Tree<T>{
	TreeNode<T> root;
	class Treenode<T>{
		T element;
		TreeNode<T> firstChild;
		TreeNode<T> nextSibling;
		TreeNode<T> parent;
	}
}
```

### Tree Traversal
##### Depth First
preorder - visit the root first then child
```java
depthFirst (root){
	if (root is not empty) {
		visit root
		for each child of root
			depthFirst(child)
	}
}
```
postorder - visit the child than the root
- height is computed with postorder
- number of bytes in a tree
- 