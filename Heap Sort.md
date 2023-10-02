
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

# Construction of MAX heap
- Check if every non-leaf node has number greater that its child nodes. IF not - swap.

# Insertion
- Insert element as last leaf node.
- Repeat Construction method

# Deletion
- Delete element.
- Replace it with the last leaf node.
- Repeat Construction method.

# Sort
- create heap from given array.
- Based on MAX or MIN heap, top element would be MAX or MIN. (assuming max heap here).
- Delete the MAX and heapify again.
- This will give second MAX. 
- Rinse and Repeat until heap is empty
![[Pasted image 20231003003517.png]]
