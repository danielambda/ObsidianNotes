---
id: evolutionary-algorithm:2024-12-03-01-57-38
aliases:
  - Evolutionary Algorithm
tags: []
---
# Evolutionary Algorithm

## Pseudo Code
- Create a randomized **population** made up of **chromosomes** (data structures encoding a potential solution)
- Until **success criteria** is met
  - Find an **fitness score** for each member of the population
  - Select members to act upon using some **variation operators**
    - Apply operations on the members
      - **Crossover**
      - **Mutations**
  - Replace some member of the population with these children from the variation operators
  - Keep some members from the previous population in the new population, i. e. **elitism/inheritance**
