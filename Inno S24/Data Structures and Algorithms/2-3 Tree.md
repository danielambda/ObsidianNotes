---
tags:
  - DataStructures
  - GraphTheory
---
## Invariants
- 2-3 Tree is a type of self-balancing search tree
	1. Each internal node has either 2 or 3 children
	2. All leaves are at the same level
	3. It is a search [[Tree]]
## Insertion
- The idea for insertion is simple:
	1. Insert a new value in a leaf node
	2. If node has 3 values
		1. Promote the middle value to restore balance
		2. Continue recursively to the top, until the entire is balanced
## Deletion 
- The idea for deletion is simple
	1. Delete a value using the [[Binary Search Tree|default search tree deletion]]
	2. If we end up with an empty leaf:
		1.  If possible, transfer (redustribute) to fix locally
		2. Otherwise, perform fusion (merge) and continue recursively
## Transfer (redustribute)
![[Pasted image 20240314125658.png]]
## Fusion (merge)
![[Pasted image 20240314125812.png]]
