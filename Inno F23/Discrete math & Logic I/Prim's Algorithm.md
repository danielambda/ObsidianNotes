---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "11.50"
---
## Algorithm
1. We start from a single vertex, chosen from the [[Graph]]
2. Grow the tree $T$ by one edge:
	- Find the edges that connect $T$ to vertices not yet in $T$
	- Choose from them the minimum-weight edge
	- Transfer it to $T$
3. Repeat step 2 until all vertices are in the tree $T$