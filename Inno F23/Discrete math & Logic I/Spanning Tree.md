---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "11.28"
---
## Definition
Let $G=(V,E)$ be a connected [[Graph]]. A graph $G'=(V,E')\subseteq G$ is called a *spanning tree* if $G'$ is a [[Tree]]
## Theorem
- ### Statement
	Any connected [[Graph]] has a spanning tree
- ### Proof
	Let $G$ be a connected [[Graph]]
	- #### Algorithm to Find some Spanning Tree
		- Repeat the following procedure:
	for $i=1,2,...$ as long as possible
	If $G$ contains a [[Walk|cycle]], remove one edge from the [[Walk|cycle]] 