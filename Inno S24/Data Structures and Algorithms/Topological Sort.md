---
tags:
  - Math
  - Algorithms
  - DataStructures
  - GraphTheory
---
## Definition
- A linear ordering of vertices such that
	- for every edge $U\to V$
		- vertex $U$ comes before $V$ in the ordering
## Kahn's Algorithm
```
while S is not empty do
	remove node n from S
	add n to L
	foreach node m with an edge from n to m do
		remove edge e from the graph
		if m has no other incoming edges then
			insert m into S

if graph has edges then
	return error
else
	return L
```