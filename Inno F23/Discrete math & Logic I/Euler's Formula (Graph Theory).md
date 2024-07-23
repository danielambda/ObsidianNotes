---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "13.9"
---
## Theorem
- Let $G$ be a connected [[Planar Graph]], $P(G)$ be any plane of its embeddings. Then: $$v-e+f=2$$ $$В-Р+Г=2$$
- where 
	- $f$ is the number of faces of $P(G)$
	- $v$ is the number of vertices
	- $e$ is the number of edges of $G$
## Proof 
### by induction on the number of faces $f$
- #### Base
	- If $f = 1$ then the graph is a tree. The claim holds
- #### Hypothesis
	- Suppose that the claim is true for all plane embeddings with less then $f$ faces for $f\geq2$
- #### Step
	- Let $P(G)$ be a plane embedding of a connected [[Planar Graph]] $G$ such that $P(G)$ has $f\geq2$ faces
	- Let $e$ be an edge that lies in some [[Walk|cycle]].
	- $G-e$ is planar and $P(G-e)$ has $f-1$ faces because the two faces of $P(G)$ that are separated by $e$ are merged into one face of $P(G-e)$
	- By hypothesis: $v_{G-e}-e{G-e}+(f-1)=2\implies v_G-(e_G-1)+(f-1)=2$
- #### Conclusion
	- The statement is true for all $f$
## Corollary 1
- ### Statement
	- If $G$ is a [[Planar Graph]]: $v_G\geq3\implies e_G\leq 3v_G-6$
- ### Proof
	- Each face contains at least three edges on its boundary
	- Each edge lies on at most two faces
	- Hence $3f_G\leq2e_G$
	- Therefore, $3(e_G-v_G+2)\leq2e_G\implies e_G\leq3v_G-6. \blacksquare$
## Corollary 2
 - ### Statement 
	 - $K_5$ is not a [[Planar Graph]]
- ### Proof
	- $v=5,e=10$
	- By corollary 1:
		- $10\leq3*5-6=9$ - false
		- Therefore, $K_5$ is not a [[Planar Graph]]. $\blacksquare$
### Corollary 3
- ### Statement
	- $K_{3,3}$ is not a [[Planar Graph]]
- ### Proof
	- $v=6,e=9$
	- Since $K_{3,3}$ is a bi-graph, each face contains at least $3+1=4$ edges on its boundary.
	- Hence, $f_G\leq2e\iff4\times5\leq2\times9$ - false
	- Therefore, $K_{3,3}$ is not a [[Planar Graph]]. $\blacksquare$