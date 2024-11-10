#comp250 
Partition a list into sublists recursively until sublists sorted which are then merged back together

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