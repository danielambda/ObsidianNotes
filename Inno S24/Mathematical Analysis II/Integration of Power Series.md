---
tags:
  - Math
  - MathematicalAnalysis
---
## Theorem about Integrating of the [[Power Series]]
- The [[Theorem about the Radius of Convergence|Radius of Convergence]] $R$ does not change for term by term integrated [[Power Series]]
## Proof
- Consider term by term [[Antiderivative]] of the series:
$$\sum_{n=0}^\infty\int a_nx^ndx=\sum_{n=0}^\infty\frac{a_n}{n+1}x^{n+1}$$
$$\lim_{n\to\infty}\sqrt[n]{\left|\frac{a_n}{n+1}\right|}=\frac{\displaystyle\lim_{n\to\infty}\sqrt[n]{|a_n|}}{\displaystyle\lim_{n\to\infty}\sqrt[n]{n+1}}=\frac{\frac{1}{R}}{1}=\frac1R\implies R(S'(x))=R(S(x)). \blacksquare$$
## Corollary
$$S(x)=\sum_{n=0}^\infty a_n\frac{x^{n+1}}{n+1}=\implies S'(x)=\sum_{n=0}^\infty a_nx^n$$
- Let $R$ be the [[Theorem about the Radius of Convergence|Radius of Convergence]] for the [[Power Series]]:
- For $$\forall\alpha, \beta\in\mathbb R: -R<\alpha<\beta<R\implies\int_\alpha^\beta\sum_{n=0}^\infty a_n x^n dx=\sum_{n=0}^\infty\frac{a_n}{n+1}(\beta^n-\alpha^n)$$