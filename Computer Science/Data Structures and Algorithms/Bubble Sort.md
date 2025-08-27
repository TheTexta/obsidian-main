#comp250 
- Simplest [[sorting algorithms|sorting algorithm]]
- Repeatedly iterate through the list and swap adjacent elements if in the wrong order
- largest ele goes to the end after first it.

```psuedocode
i=0
sorted = false
while (!sorted) {
	sorted = true
	for j from 0 to list.length -2 -i {
			if (list[j]>list[j+1]){
				swap(list[j],list[j+1])
				sorted=false
			}
		}
	i++
}
```