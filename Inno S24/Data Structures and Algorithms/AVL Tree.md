---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
  - DataStructures
---
## Definition
- An AVL Tree is a [[Binary Search Tree]] that is **height balanced**:
	- For each node the heights of its subtrees differ by at most 1
### Note:
- Implementations of AVL trees maintain an extra attribute in each node (e.g. $x.h$ as the height of the node $x$)
## Insertion
- To insert into an AVL tree, we first place a node into the appropriate place in [[Binary Search Tree]] order. Afterward, the tree might no longer be height balanced. Specifically, the heights of the left and right children of some node might differ by 2. Then you have to rebalance it somehow using [[BST Rotations]]