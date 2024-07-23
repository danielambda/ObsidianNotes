---
tags:
  - Math
  - Combinatorics
  - DiscreteMath
  - Logic
---
## Definition
- Let $x, y$ be variables, $n \geq 1$ be a natural number. Then: $$\large(x+y)^n=\sum^n_{j=0}\left(\begin{matrix} n \\ j\end{matrix}\right)x^{n-j}y^j$$
## Example
$\large(x+y)^3=\binom{3}{0}x^3+\binom{3}{1}x^2y+\binom{3}{2}xy^2+\binom{3}{3}y^3 = x^3+3x^2y+3xy+y^3$
## Proof (by induction)
### Base
- Let $n = 1.\;\large(x +y)^1=\binom{1}{0}x+\binom{1}{1}y$
### Hypothesis
- Suppose that for $k\in\mathbb N:$ $$\large(x+y)^k=\sum^k_{j=0}\binom{k}{j}x^{k-j}y^j$$
### Step
We need to prove
$$\displaystyle (x+y)^{k+1}= \sum^{k+1}_{j=0}\binom{k+1}{j}x^{k+1-j}y^j$$
$\displaystyle (x+y)^{k+1}=(x+y)^{k}(x+y) =\left(\sum^k_{j=0}\binom{k}{j}x^{k-j}y^j\right)(x+y)=$
$\displaystyle\sum^k_{j=0}\binom{k}{j}x^{k+1-j}y^j + \sum^k_{j=0}\binom{k}{j}x^{k-j}y^{j+1}=\sum^k_{j=0}\binom{k}{j}x^{k+1-j}y^j + \sum^{k+1}_{j=1}\binom{k}{j-1}x^{k+1-j}y^{j}=$
$\displaystyle=\binom{k}{0}x^{k+1}y^0+\sum^k_{j=1}\left(\binom{k}{j}+\binom{k}{j-1}\right)x^{k+1-j}y^j + \binom{k}{k}x^0y^{k+1}=$
$\displaystyle=x^{k+1}y^0+\sum^k_{j=1}\binom{k+1}{j}x^{k+1-j}y^j + x^0y^{k+1} = \sum^{k+1}_{j=0}\binom{k+1}{j}x^{k+1-j}y^j, Q.E.D.\blacksquare$
### Conclusion
By mathematical induction, since the fact that statement​ is true for $n=1$ and so is statement for $k$​ implies statement for $k+1$​ is true, statement is true for all positive integers $n$.
## Corollary
$$\displaystyle\sum^n_{j=0}\binom{n}{j}=(1+1)^n=2^n$$
$$\sum^n_{j=0}\binom{n}{j}(-1)^j=(1+(-1))^n=0$$