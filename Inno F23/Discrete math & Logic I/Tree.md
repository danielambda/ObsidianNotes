---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "11.5"
---
## Definition
A connected undirected simple [[Graph]] having no [[Walk|cycle]] is called a *tree*
	or
A connected [[Forest]] is called a *tree*
## Equivalent Definitions
The following are equivalent for a graph $T$:
1. $T$ is a *tree*
2. any two vertices of $T$ are connected by a unique [[Walk|path]] is $T$
3. $T$ is minimally connected
	- $T$ is connected
	- $T-e$ is no connected for any of its edge $e$
4. $T$ is maximally acyclic
	- $T$ contains no [[Walk|cycles]]
	- $T+(x,y)$ contains a [[Walk|cycle]] for any two non-[[Graph|adjacent]] vertices $x,y\in V_T$ 
## The Characteristic Property
Let $G$ be a connected [[Graph]] with $n$ vertices and $e$ edges.
$$G\;is\;a\;tree\iff n=e+1$$
- ### Proof (by induction)
	- #### Base
		- Let $n=1\implies e=0$. Obvious
	- #### Hypothesis
		- Suppose $\forall k:k=e+1$
	- #### Step
		- Let $G$ be a [[Tree]] with $n=k+1$ vertices and $e_G$ edges.
			- Chose a vertex $v$ with degree of 1 ([[Any Tree has 2 Vertices with Degree 1]])
			- Then $G-v$ is a [[Tree]] with $k$ vertices
			- Therefore, (by the induction hypothesis) $G-v$ has $e_{G-v} = k-1$ edges, i.e., $k=e_{G-v}+1$
			- Return the vertex and the edge: $n=e_G+1$
			- Suppose that $G'=(V_G,E')\subseteq G$ is a [[Tree]] ($G'$ is a [[Spanning Tree]])
			- Since $G'$ has $n$ vertices and $n-1$ edges, and $G$ has $n$ vertices and $n-1$ edges, 
				by the first implication $\implies G'=G$
				