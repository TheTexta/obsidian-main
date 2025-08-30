#comp250 

```java
System.out.println(1+2+"A"+3+4) -> 3A34
System.out.println((new int[5])[3]) -> 0
double x == double y // shouldnt be compared like this instead through abs diff of.
while (node != null && node.next != null){
	swap(node, node.next);
	node = node.next.next;
}
```

- declare class methods appropriately (public and static)
- hashcode doesnt tell us anything about the content
- arraylists have to have items to use .set()
- lil uml diagram - variables in top methods in bottom
- doubles should be compared through math.abs()
```plantuml
class Food{
+ consumed
}
class Dessert extends Food {
+ isCold():boolean
}

```
- ``ArrayList<Wizzard> slytherin = new Arraylist<Wizzard>();`` - creates 2 objects - ArrayList and Wizzard[]
- This one is pretty weird - ![](../../assets/screenshots/IMG_3624.png)

##### Sorting Algorirthms
Selection Sort
```java
for delim from 0 to N-2 {
	min = delim
	for i from dleimn + 1 to N-1 {
		if (list[i]<list[min]){
			 min = i}}
	if (min != delim){
		swap(list[min], list[delim])}}
```

Bubble Sort
```java
i=0
sorted = false
while (!sorted) {
	sorted = true
	for j from 0 to list.length -2 -i {
			if (list[j]>list[j+1]){
				swap(list[j],list[j+1])
				sorted=false}}
	i++}
```

Insertion Sort
```java
for i from 0 to N-1 {
	element = list[i]
	k=i
	while (k>0&&element<list[k-1]){
		list[k]=list[k-1]
		k--}
	list[k]=element}
```