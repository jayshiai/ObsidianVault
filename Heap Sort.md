
 ![[Pasted image 20231003000738.png]]
 - Array representation of Heap
 - If array begins at index 0
	- Parent node - `arr[(i-1)/2]`
	- Left Most child node - `arr[2i +1]`
	- Right Most Child Node - `arr[2i + 2]`
- If index 1
	- Parent node - `arr[i/2]`
	- Left Child - `arr[2i]`
	- Right Child - `arr[2i+1`
- If all Numbers are descending - MAX tree
- If all numbers are ascending - MIN tree