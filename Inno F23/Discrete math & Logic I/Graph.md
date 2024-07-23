---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
---
## Definition (undirected simple)
A [[Ordered Pair|pair]] $G=(V,E)$ is called a *graph* if 
$$E\subseteq\{\{u,v\}|u,v\in V\;\&\;u\not=v\}$$
## Definitions
1. Two vertices $x,y$ of $G$ are *adjacent* or *neighbors* if $xy$ is an edge of $G$
2. A vertex $v$ is *incident* with an edge $e$ if $v\in e$, that is $e=(v,\cdot)\lor(\cdot,v)$
3. Two vertices incident with an edge are its *end vertices* or *ends*
4. Two edges $v,w$ of $G$ are *adjacent* or *neighbor* if one of their ends is the same
5. *Face* of a plane graph is a region bounded by edges including infinitely large outer region (exterior face)
## Neighbors
The set of neighbors of a vertex $v$ in $G=(V_G,E_G)$ is denoted by $N_G(V)$
## Degree
The degree (or valency) $d_G(v)=d(v)$ of a vertex $v$ is the number of its neighbors: $$d_G(v)=|N_G(v)|$$