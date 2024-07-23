---
tags:
  - Math
  - MathematicalAnalysis
---
## Just some Fact
- Consider $R$ is the [[Theorem about the Radius of Convergence|Radius of Convergence]]
$$\forall x\in\mathbb R: |x|< R:S(x)=\sum_{n=0}^\infty a_nx^n\implies S'(x)=\sum_{n=0}^\infty na_nx^{n-1}$$
## Theorem
- The [[Theorem about the Radius of Convergence|Radius of Convergence]] $R$ does not change for the term by term differentiated [[Power Series]]
## Proof
$$\sum_{n=0}^\infty\frac{d}{dx}(a_nx^n)=\sum_{n=0}^\infty na_nx^{n-1}$$
$$\left(\lim_{n\to\infty}\log(\sqrt[n]n)=\lim_{n\to\infty}\frac{\log(n)}{n}=0\implies \lim_{n\to\infty}\sqrt[n]{n}=1\right)$$
$$\lim_{n\to\infty}\sqrt[n]{n|a_n|}=\lim_{n\to\infty}\sqrt[n]{n}\lim_{n\to\infty}\sqrt[n]{|a_n|}=\frac1 R\implies R(S'(x))=R(S(x)). \blacksquare$$
