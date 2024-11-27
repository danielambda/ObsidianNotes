## Definitions / Formulas for First Moment ([[Expected Value]])
$$
  \mathbb E \xi = \int_{-\infty}^{+\infty}x p_\xi(x)\,dx
$$
$$
  \mathbb E \xi = -\int_{-\infty}^{0} F_\xi (x)dx + \int_{0}^{+\infty}(1 - F_\xi(x)) dx
$$

## $g(\xi)$
- Let $\xi$ be a [[Continuity|continuous]] [[Random Variable]] with [[1728426412-probability-density-function|pdf]] $p_\xi$, and let $g: \mathbb R\to\mathbb R$ be a measurable [[Function]].
- Then for the [[Random Variable]] $g(\xi)$ its [[Expected Value]] is:
$$
   \mathbb E g(\xi) = \int_{-\infty}^{+\infty} g(x) p_\xi (x)\,dx
$$

#### Examples
1. This fact can be used in [[Moment Generating Function|Moment-Generating Function]]

2. Let us find the [[Expected Value]] and [[Variance]] of a [[Random Variable]] $\xi\sim\mathcal N(0,1)$
   $$
      \mathbb E \xi = \int_{-\infty}^{+\infty} x \frac{1}{\sqrt{2\pi}}e^{\frac{-x^2}{2}}dx = 0
   $$
   it is 0 because integrating odd function from $-\infty$ to $+\infty$
   - Compute the second moment:
   $$
      \mathbb E \xi^2 = \int_{-\infty}^{+\infty} x^2 \frac{1}{\sqrt{2\pi}}e^{\frac{-x^2}{2}}dx = ... = 1
   $$
   - Therefore, $\text{Var }\xi = \mathbb E\xi^2 - (\mathbb E \xi)^2 = 1 - 0 = 1$
