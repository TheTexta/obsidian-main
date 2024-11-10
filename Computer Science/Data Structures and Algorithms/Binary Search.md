#comp250 
Inputs:
- A sorted list
- The element we looking for - the key

IDEA: First compare the key with the element in the middle of the list
- If the key is less than the middle element we only need to search the first half of the list
- If greater then we continue on the second half
- With one element or an empty list we compare and result is either *found* or *not found*
- Use indices left and right to keep track of where in the list is still viable


```java
binarySearch(list, key, left, right){
	if (left<=right){
		mid = (left+right) / 2
		if (list[mid]==key){
			return mid;
		} else {
			if (key<list[mid])
				return binarySearch(list,key,min,mid-1);
			else
				return binarySearch(list,key,mid+1,mid);
		}
	}
	return -1;
}
```