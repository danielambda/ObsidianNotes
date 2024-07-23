---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "14.19"
---
## Definition
- For a [[Transportation Network]] $N=(V,E,c,s,t)$ a *cut* is a set $C\subseteq E$ such that there are sets $S,T$ with
$$C=\{\overline{(u,v)}\in E|u\in S\;\&\;v\in T\}$$
$$S\cup T=V, S\cap T=\emptyset$$
$$s\in S, t\in T$$
- The capacity of a cut $C$ is the sum of $c(e)$ for $e\in C$ $\left(\displaystyle\sum_{e\in C}c(e)\right)$