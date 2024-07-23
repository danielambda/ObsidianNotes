---
tags:
  - DataStructures
  - Algorithms
---
## Operations
```
insert(key, value) - insert a key-value pair into a heap
minimum() - get the minimum key from the heap
extractMin() - remove and return the minimum key from the heap
union(anotherHeap) - combine two heaps, containint all elements from the current one and anotherHeap

//additionally
decreasyKey(newValue, key) - update the key of new value, assuming new value is not greater than current value, and newValue is a direct reference to an entry in the heap
delete(entry) - remove from heap
```
## [[Binary Heap]] vs Fibonacci Heap
![[Pasted image 20240314131005.png]]
## Structure of a Fibonacci Heap
- A collection of min-heap trees with tracked minimum
![[Pasted image 20240314131113.png]]
## Insertion
-  Simply add a singleton min-heap tree to the root list
## Extracting Minimum
1. Delete min node, and add its children to the root list
2. Consolidate the root list recursively:
	- find two roots with the same degree and link them (to keep track of degrees, we can utilize an array)
## Decrease Key
1. Decrease the key
2. If heap property is violated -- move the entire subtree to the root list
3. Mark the parent as "loser" as its lost its subtree
4. If parent is already a "loser", move it also to the root list (with the remaining subtrees attached), and inspect grandparent similarly