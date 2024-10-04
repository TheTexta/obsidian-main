#comp250 
- List as two parts, one sorted and other unsorted
- best and worst case same op time
- procedure
	- select the smallest element in the unsorted list
	- swap with element in initial position of sorted array
	- change where you divide the array from the sorted part to the unsorted part
	- tldr: bring the smallest unsorted element forward and increase the delimeter by one.

```psuedocode
for delim from 0 to N-2 {
	min = delim
	for i from dleimn + 1 to N-1 {
		if (list[i]<list[min]){
			 min = i
		}
	}
	if (min != delim){
		swap(list[min], list[delim])
	}
}
```