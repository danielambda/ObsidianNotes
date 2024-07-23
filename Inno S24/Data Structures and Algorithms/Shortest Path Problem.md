---
tags:
  - Math
  - DataStructures
  - Algorithms
  - GraphTheory
  - Optimization
---
## Definition
- Given a weighted [[Graph]] $G=(V,E)$ and two vertices $u$ and $v$, we want to find a [[Walk|path]] of smallest total weight from $u$ to $v$.
## Applications:
1. Network packet routing 
2. Flight reservations
3. Driving directions
4. Planning
5. …
## Terminology 
- Input to a shortest path problem:
	- a weighted, directed graph $G=(V,E)$
	- with a weight function $w: E\to\mathbb R$
- A shortest path weight $\delta(u,v)$ from $u$ to $v$ is defined as:
	- $\delta(u,v)=\min\set{w(p),\forall p\text{ from } u\text{ to } v}$, if $\exists p$ from $u$ to $v
	- $\delta(u,v)=\infty,$ otherwise
- A shortest path from $u$ to $v$ is any path $p: w(p)=\delta(u,v)$
## Properties of Shortest Paths
- Triangle inequality
	- $\delta(s,v)\leq\delta(s,u)+w(u,v)$
- Upper-bound property
	- $v.ShortestPathWeight \geq \delta(s,v)$
- No-path property
	- $v.ShortestPathWeight=\delta(s,v)=+\infty$ for unreachable vertices
- Convergence property
	- If $s\to u\to v$ is the shortest path, and $u.ShortestPathWeight=\delta(s,u)$
		- then after relaxing edge from $u$ to $v$, we have $v.ShortestPathWeight=\delta(s,v)$