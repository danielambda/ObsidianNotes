---
tags:
  - Math
  - DataStructures
  - DiscreteMath
  - GraphTheory
---
## Definition
- [[k-ary Tree]] for $k=2$
- A binary tree of size $n$ either
	-  is an empty [[Tree]] if $n = 0$
	- or has a root node $u$ and two binary subtrees $l, r$ of sizes $n_1,n_2$ such that $n= 1 + n_1+n_2$
## Linked Representation
![[Pasted image 20240304210616.png]]
## Array Representation
- To represent a tree in an array we need 
	1. A way to assign positions in array to nodes in a tree
	2. A way to compute position of a parent from a position of a child
	3. A way to compute position of children from a position of a parent
--- 
$$\displaystyle\large p(root)=0, p(parent)=\left\lfloor\frac{p(child)-1}{2}\right\rfloor$$
$$\large p(left)=2\cdot p(parent)+1, p(right)=2\cdot p(parent)+2$$