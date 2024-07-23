---
tags:
  - Math
  - DataStructures
  - Algorithms
  - AsymptoticAnalysis
---
## Theorem
- Let $a>0, b>0$ be constants, and let $f(n)$ be a driving function that is defined and nonnegative on all sufficiently large reals. Define the recurrence $T(n)$ on $n\in\mathbb N$ by $$T(n)=aT\left(\frac nb\right)+f(n)$$
- where $\displaystyle aT\left(\frac nb\right)$ actually means $\displaystyle a'T\left(\left\lfloor\frac nb\right\rfloor\right)+a''Ta'\left(\left\lceil\frac nb\right\rceil\right)$ for some constants $a', a''\geq 0, a'+a''=a$. Then the asymptotic behavior of $T(n)$ can be characterized as follows:
1. If there exists a real positive constant $\varepsilon$ such that $f(n)=O(n^{\log_ba-\varepsilon})$, then 
	$$T(n)=\Theta(n^{\log_ba})$$
2. If there exists a real nonnegative constant $k$ such that $f(n)=\Theta(n^{\log_ba}\lg^kn)$, then $$T(n)=\Theta(n^{\log_ba}\lg^{k+1}n)$$
3. If there exists a real positive constant $\varepsilon$ such that $f(n)=\Omega(n^{\log_ba+\varepsilon})$, and if $f(n)$ additionally satisfies the *regularity condition* $$\exists N\in\mathbb N\;\forall n\in\mathbb N, n>N\;\exists c\in\mathbb R, c<1:af\left(\frac nb\right)\leq cf(n)$$ then $$T(n)=\Theta(f(n))$$
## Cases but formal
$$1. \exists\varepsilon\in\mathbb R,\varepsilon>0:f(n)=O(n^{\log_ba-\varepsilon})\implies T(n)=\Theta(n^{\log_ba})$$

---
$$2.\exists k\in\mathbb R, k\geq0: f(n)=\Theta(n^{\log_ba}\lg^kn)\implies T(n)=\Theta(n^{\log_ba}\lg^{k+1}n)$$

---
$$3.\left(\left(\exists\varepsilon\in\mathbb R,\varepsilon>0: f(n)=\Omega(n^{\log_ba+\varepsilon})\right)\;\&\;\right.$$
$$\left.\left(\exists N\in\mathbb N\;\forall n\in\mathbb N, n>N\;\exists c\in\mathbb R, c<1:af\left(\frac nb\right)\leq cf(n)\right)\right)\implies$$
$$T(n)=\Theta(f(n))$$
## Important!!
- Cases are exclusive, so, if one case is applied, then others cannot be.