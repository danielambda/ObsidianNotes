---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "13.26"
---
## Definition
- A $k$-*coloring* of a [[Graph]] $G$ is a mapping $\alpha:V_G\to\{1..k\}$
- The *coloring* $\alpha$ is proper if adjacent vertices have different colors:
$$\forall vv'\in E_G:\alpha(v)\not=\alpha(v')$$
- A [[Graph]] $G$ is $k$-colorable if there is a proper $k$-coloring for $G$
- [[Chromatic Number]] 
## Theorem
- The following are equivalent:
	1. $\chi(G)=2$
	2. $G$ is a non-trivial bi-graph
	3. All [[Walk|cycles]] of $G$ have even number of edges