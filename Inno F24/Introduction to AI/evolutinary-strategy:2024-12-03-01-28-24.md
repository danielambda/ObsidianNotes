---
id: evolutionary-strategy:2024-12-03-01-28-24
aliases:
  - Evolutionary Strategy
tags: []
---
# Evolutionary Strategy

#### Representation
- [[Vector]] of real number

#### Selection
- Replace with a mutation sample member if it is better than parent

#### Crossover
- Unnecessary, but can be used

#### Mutation
- Add small [[normal-distribution:2024-12-03-01-34-17|normally distributed]] parameter to a value

## Variants of Mutation
1. $(1+1)$ - a mutant is tested against its parent and the fittest is retained
2. $(1+\lambda)$ - $\lambda$ mutants are tested against their parent and the fittest is retained
3. $(1, \lambda)$ - $\lambda$ mutants are tested against their parent, but the parent is never retained, only one of mutants will continue
4. $(\mu/\rho, \lambda)$ - a population is used where a group of mutants is made for each and complete with the set of parents, this may also have a crossover operation

