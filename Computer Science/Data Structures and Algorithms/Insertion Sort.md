#comp250 
- consider the list as if it was divided into two parts, one sorted and the other unsorted.
- $T_\text{worst}(n)=an^2+bn+c$ therefor the function is upper bounded by [[big O]] $O(n^2)$
- $T_\text{best}(n)=an+b$ where $a$ and $b$ are some constants. $\Omega (n)$ is the [[big omega]] of n


### Procedure
- select the first element of the unsorted part of the list
- insert such element into its correct position in the sorted part of the list
- change where you divide the array from the sorted part to the unsorted part

### Implementation
```pseudocode
for i from 0 to N-1 {
	element = list[i]
	k=i
	while (k>0&&element<list[k-1]){
		list[k]=list[k-1]
		k--
	}
	list[k]=element
}
```