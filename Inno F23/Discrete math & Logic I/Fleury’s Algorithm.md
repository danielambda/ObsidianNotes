---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "12.37"
---
## Purpose
- The purpose of the Algorithm is to find [[Euler Cycle]] or [[Euler Path]] is a [[Graph]] is there is such.
## Algorithm
1. Let $v_0$ be an arbitrary vertex, and $W_0=\emptyset$
2. Repeat the following procedure for $i=1,2...$ as long as possible:
	1. Suppose that $W_i=\{e_1,e_2,...,e_i\}$ has been constructed, where $e_j=(v_{j-1},v_j)$. Choose a new edge $e_{i+1}$ such that
		1. $e_{i+1}\not\in W_{i}\;\&\;v_i\in e_{i+1}$
		2. $G-\{e_1,e_2,...,e_i,\color{red}e_{i+1}\color{white}\}$ does not contain two non-trivial connected components, unless there is no alternative