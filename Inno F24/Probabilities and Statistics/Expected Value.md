---
aliases: First Moment
---

## Definition
- Expected value (first moment) of a random variable $\xi$ is:
$$
  \mathbb E \xi = -\int_{-\infty}^{0} F_\xi (x)dx + \int_{0}^{+\infty}(1 - F_\xi(x)) dx
$$
where
- $F_\xi(x)$ is [[Cumulative Distribution Function]]

## For Discrete [[Random Variable]]
$$
  \mathbb E \xi = \sum_{x \in X}^{} x \cdot p_\xi(x)
$$
where
- $X$ is the set of all the values that $\xi$ can take
- $p_\xi x$ is a [[Probability Mass Function]] of $\xi$

## For [[Continuity|Continuous]] [[Random Variable]]
$$
  \mathbb E \xi = \int_{-\infty}^{+\infty}x p_\xi(x)\,dx
$$
where
- $p_\xi x$ is a [[1728426412-probability-density-function|Probability Density Function]]
