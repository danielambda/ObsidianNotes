---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
---
## Statement
Any [[Tree]] has a vertex with degree 1 (even any non-trivial tree has at least 2 such vertices)
## Proof
- Since $G$ is a [[Tree]], $G$ is connected.
- Let $v_0,v_1,...,v_{n-1},v_n$ be a path of maximum length
- Then $v_0, v_n$ cannot be [[Walk|adjacent]] to any other vertices in $G$ not on $P$ because then we could extend $P$ to a longer path in $G$.
- Neither $v_0$ nor $v_n$ can be [[Walk|adjacent]] to any other vertices in $P$ other than $v_1$ and $v_{n-1}$ because that would induce a [[Walk|cycle]] in $G$, which contradicts to the assumption that $G$ is a [[Tree]].
- Thus, $deg(v_0)=1\;\&\;deg(v_n)=1$
