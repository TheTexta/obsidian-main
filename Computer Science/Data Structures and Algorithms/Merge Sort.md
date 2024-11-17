#comp250 
Partition a list into sublists recursively until sublists sorted which are then merged back together

$O(n\cdot \log {n})$

```java
mergeSort(list){
	if (list.size()<=1)
		return list
	else {
		mid = (list.size()-1)/2
		list1=list.getElements (0,mid);
		list2 = list.getElements (mid+1,list.size()-1)
		list1 = mergeSort(list1);
		list2 = mergeSort(list2);
		return merge (list1,list2); // merge is where the sorting happens with dual pointers
	}
}
```

```java
merge(list1,list2){
	list = new list;
	while (!list1.isEmpty && !list2.isEmpty){
		if (list1.get(0)<list2.get(0)){
			list.addlast(list1.removeFirst())
		} else {
			list.addlast(list2.removeFirst())
		}
	}
	while (!list1.isEmpty())
		list.addlast(list1.removeFirst())
	while (!list2.isEmpty())
		list.addlast(list2.removeFirst())
	return list
}
```

### Complexity/runtime
$T(1)=a$
$T(n)=b+c\cdot n + 2\cdot T(\frac{n}{2})$
$T(n)=cn + 2 \left( c\frac{n}{2} + 2T\left(\frac{n}{4}\right) \right) = cn + cn + 4T\left(\frac{n}{4}\right)$
$T(n)=k\cdot cn+2^k\cdot T(\frac{n}{2^k})$
k such that n/2^k =1
$k=log_2(n)$
$T(n)=log_2(n)\cdot cn + 2^{log_2(n)}\cdot T(1)$
$T(n)=cnlog_2(n)+bn$
which is $\Theta(n\log n)$

