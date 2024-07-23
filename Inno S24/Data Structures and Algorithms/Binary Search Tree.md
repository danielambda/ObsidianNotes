---
tags:
  - Math
  - DataStructures
  - DiscreteMath
  - GraphTheory
---
## Definition
- A [[Binary Search Tree]] (BST) is a [[Binary Tree]] that allows efficient search.
- The keys in a BST satisfy a binary search tree property
## Binary search tree property
- For any node $x$ in a BST
	1. If $y$ is a node in the left subtree of $x$, then $y.key\leq x.key$
	2. if $y$ is a node in the right subtree of $x$, then $y.key\geq x.key$
## Supported Operations
```
search(key)
add(item)
remove(item) or remove(key)
removeMax()
removeMin()
findMax()
findMin()
```
## Recursive Search
``` C#
Node TreeSearch(Node x, int k) 
{
	if (x is null || k == x.Key)
		return x;

	if (k < x.key)
		return TreeSearch(x.Left, k);

	return TreeSearch(x.Right, k);
}
```
## Iterative Search
```C#
Node IterativeTreeSearch(Node x, int k) 
{
	while (x is not null && k != x.Key) 
	{
		if (k < x.key)
			x = x.Left;
		else
			x = x.Right;
	}

	return x;
}
```
## Insertion
- To insert into a [[Binary Search Tree]]: 
	1. Search for the place for the key in a [[Binary Tree]]
	2. Insert element as a leaf at the node where the search ended
## Deletion
- To delete from a [[Binary Search Tree]]:
	1. Search for the node to remove
	2. If the node is not found - return
	3. If the node is a leaf -- remove it
	4. If the node has one child
		- Remove the node
		- Attach the subtree instead of the deleted node to its parent
	5. If the node has two children:
		- Exchange the node with a successor (or a predecessor) node
		- Recursively remove the node from its new place
![[Pasted image 20240304212952.png]]
