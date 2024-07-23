---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
  - Programming
  - DataStructures
  - Algorithms
slide: "13.32"
---
## Description
- The algorithm starts at selecting some arbitrary edge and explores as far as possible along each branch before backtracking.
## Algorithm with [[Stack]]
1. Push the starting node onto the Stack
2. Visit current node (node at the top of the Stack)
3. Mark current node visited
4. If possible, continue from an adjacent unvisited node
5. Otherwise, backtrack by popping from the Stack (or stop when empty)
## Time Complexity
- $O(|V|+|E|)$