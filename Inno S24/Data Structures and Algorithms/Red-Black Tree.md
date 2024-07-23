---
tags:
  - Math
  - DataStructures
  - GraphTheory
---
## Invariant
- Red-Black Tree is a type of self-balancing [[Binary Search Tree]]
	1. Each node is either $\color{red}red$ or $\color{grey}black$ (information is stored in each node)
	2. The root is always $\color{grey}black$
	3. Every leaf (Null) is $\color{grey}black$
	4. If a node is $\color{red}red$, then both its children are $\color{grey}black$
	5. For each node, all paths from this node to any leaf contain the same number of $\color{grey}black$ nodes
## Insertion
- The idea for insertion:
	1. Insert a new $\color{red}red$ node using the default [[Binary Search Tree|BST]] insertion
	2. Fix the tree recursively raising from the new node:
		1. If current node's parent is $\color{grey}black$ -- stop
		2. If current node's parent and uncle are both $\color{red} red$ -- recolor and go up (case 1)
		3. If current node's parent is $\color{red}red$ and uncle is $\color{grey}black$, then [[BST Rotations|rotate]], recolor, and go up (cases 2 and 3)
### Insertion cases:
#### case 1: 
![[Pasted image 20240304214501.png]]
#### case 2 (inserted to the edge):
![[Pasted image 20240304214527.png]]
#### case 3 (inserted into middle):
![[Pasted image 20240304214554.png]]
## Deletion
- The idea for deletion:
	1. Delete a node using the default [[Binary Search Tree|BST]] deletion
	2. If deleted node was $\color{red}red$, nothing has to be adjusted
	3. Otherwise, fix the [[Tree]] recursively raising from the deleted node:
		1. If current node is $\color{red}red$ -- stop
		2. Examine current node's sibling and nephews to perform [[BST Rotations|rotation]] and recoloring correspondingly
### Deletion cases
#### case 1 (sibling is $\color{red}red$):
![[Pasted image 20240304215130.png]]
#### case 2 (sibling is $\color{grey}black$, both nephews are $\color{grey}black$):
![[Pasted image 20240304215209.png]]
#### case 3 (sibling is $\color{grey}black$, left nephew is $\color{red}red$, right is $\color{grey}black$)
![[Pasted image 20240304215330.png]]
#### case 4
![[Pasted image 20240304215352.png]]
