---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
a.k.a.: Euler Tour, Euler Circuit
slide: "12.16"
---
## Definitions
- A [[Walk|cycle]] is called Euler, if it contains every edge and only once
- A [[Graph]] having an Euler cycle is called an *Eulerian*
## Remark
- An Euler cycle = An Euler tour = An Euler circuit
## Theorem 
### (the sufficient and necessary condition)
- A non-trivial connected [[Graph]] is Eulerian $\iff$ every vertex has even degree
### Proof ($\implies$)
- If a vertex is appearing $k$ times in a Euler cycle, then it must have degree $2k$, because we come out and come in every such vertex $k$ times. $\square$
## Proof ($\impliedby$)
- Suppose that $G$ is a non-Eulerian connected [[Graph]] with at least one edge and all vertices have even degree. 
- Since each vertex of G has degree at least 2, the G must contain a cycle.
- Since the $G$ contains a cycle, we can find a Euler cycle $C$ of maximum possible length.
- Obviously, C is itself Eulerian. So, each vertex of C has even degree.
- Therefore, each vertex of $G − E_C$ has also even degree and is not trivial (since $G$ is not an Eulerian). 
- Thus, $C$ can be extended. It [[Contradiction in Formal Logic|contradicts]] with the choice of $C$. $\square$
$\blacksquare$
## Corollary
- A connected graph has an [[Euler Path]] $\iff$ it either has no, or has exactly two vertices with odd degrees.