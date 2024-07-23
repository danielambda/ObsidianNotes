---
tags:
  - Math
  - MathematicalAnalysis
---
$M = 25 + 10 = 35$

---
# Skipped
## Task
- Indicate which of the following sequences does converge and what is the limit in this case? 
- Prove your answer for any two of these sequences using any theory covered in the lectures.
1. $\displaystyle\left(\left(1+\frac{1}{Mn}\right)^n\right)_{n\in\mathbb N,n>0}$
2. $\displaystyle\left(\left(1+\frac{1}{n}\right)^Mn\right)_{n\in\mathbb N,n>0}$
3. $\displaystyle\left(\left(1+\frac{1}{n^2}\right)^Mn\right)_{n\in\mathbb N,n>0}$
4. $\displaystyle\left(\left(1+\frac{1}{Mn}\right)^{n^2}\right)_{n\in\mathbb N,n>0}$
## Solution 1.
### Answer 1.
1. $\displaystyle\left(\left(1+\frac{1}{Mn}\right)^n\right)_{n\in\mathbb N,n>0}$ converges. $\displaystyle\lim_{n\to\mathbb N}\left(1+\frac{1}{Mn}\right)^n = e^{\frac{1}{M}}$ 
### Proof
$$\lim_{n\to\mathbb N}\left(1+\frac{1}{Mn}\right)^n = \lim_{n\to\mathbb N}\left(\left(1+\frac{1}{Mn}\right)^{Mn}\right)^\frac{1}{M}=^1$$$$=^1\left(\lim_{n\to\mathbb N}\left(1+\frac{1}{Mn}\right)^{Mn}\right)^\frac{1}{M}=^2e^{\frac{1}{M}}$$
