---
tags:
  - Math
  - Combinatorics
  - DiscreteMath
  - Logic
---
## Theorem
- The number of ways of choosing $k$ objects from $n$ types of objects (with replacement or repetition allowed) is $$\binom{n+k-1}{k}=\binom{n+k-1}{n-1}$$
- or
$$\Large\displaystyle\bar{C}_n^k = C_{n+k-1}^{k-1} = C_{n+k-1}^n = \frac{(n+k-1)!}{n!(k-1)!}$$
## Formula derivation
If we want to get number of combinations with repetitions of $k$ elements from $n$ elements we can write down $k$ ones and put $n-1$ bars between and around them. Let us say, that the set is $\{1,2,3,4,5,6,7,8\}$, $n = 8$ and $k = 5$, then we get the following: $||11|11|||1||$
This exact case corresponds to the following combination: $33447$
Every case with ones and bars corresponds to exactly one case of combinations of repetition. That means, that the number of combinations of ones and bars is equal to the number of combinations of repetitions. Since we have $k$ ones and $n - 1$ bars, the whole amount of elements is $n + k - 1$ and we have exactly $n$ bars, which means, that number of combinations of ones and bars is equal to the following binomial coefficient: $C_{n + k - 1}^n$ Q.E.D. $\blacksquare$