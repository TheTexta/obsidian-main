#comp250 

Use an array to store elements of the list and keep track of # of elements. 
# Java implementation
- uses an array as the underlying data structure
- grows the array by 50% when full and a new ele is added
- do not access fields directly - use methods provided (get(), set(), etc) to manipulate the list.
- its a generic class - you append the class type with angular brackets

```java
// initial capacity 10
ArrayList<Integer> words = new ArrayList<Integer>(); // RHS <> unnecesary with later java vs

// initial capacity 23
ArrayList<Shape> myShapes = new ArrayList<Shape>(23);
```
# Custom Implementation
### Operation time
##### Adding N elements to an array list
suppose each time we add to a full array list, we double the length of the array. Every time the array is made larger we have to copy all the elements sequentially. 

How many times k do we need to double the length of the array so that it is of length N?
$2^k=N$
$\log{2^k}=\log{N}$
$k\cdot\log{2}=\log{N}$
$k=\frac{\log{N}}{\log{2}}$
$k=\log_2{N}$

How many copy operations are required to add $N$ elements to an empty array list
$1 + 2 + 4 + ... + 2^k-1 = \sum^{k-1}_{i=0}{2^i}=\frac{1-2^k}{1-2}=2^k-1=N-1$
### Example implementation
```java
public class ArrayList {
	private Shape[] arr;
	private int size;

	public ArrayList() {
		arr = new Shape[10]; // Default size is 10 in java
		size =  0;
	}
	public Shape get(int i){
		if(i<size && i>=0)
			return arr[i];
		throw new IndexOutOfBoundsException();
	}
	public Shape set (int i, Shape e){
		if (i>=0 && i<size){
			Shape tmp = arr[i];
			arr[i]=e
			return tmp;
		}
	}
	public void add (Shape e){
		if (size==arr.length){
			resize();
		}
		arr[size]=e;
	}
	public void add (int i, Shape e){
		if (i<0)
			throw new IndexOutOfBoundsException();
		else if (i>=(size+1)){
			resize();
		}
		Shape[] tmp = arr;
		for (int j =i;j<size;j++){
			tmp[j+1]=this.get(j);
		}
		tmp[i]=e;
		arr=tmp;
	}
	private void resize(){
		Shape [] bigger = new Shape [arr.length*2];
		for (int i=0; i<size; i++){
			bigger [i] = arr[i];
		}
		arr = bigger
	}
}

ArrayList list = new ArrayList();
// add 7 elements
```