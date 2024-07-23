---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
  - Programming
  - DataStructures
  - Algorithms
slide: "13.33"
---
## Description
- The algorithm starts at selecting some arbitrary edge and explores all edges at the present depth prior to moving on to the edges at the next depth level
## Algorithm with Queue
1. Enqueue the starting node
2. Dequeue and visit the current node
3. Enqueue all its unvisited adjacent nodes
4. Continue until Queue is empty
## Time Complexity
- $O(|V|+|E|)$