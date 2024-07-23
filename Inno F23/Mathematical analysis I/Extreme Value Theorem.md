---
tags:
  - Math
  - MathematicalAnalysis
slide: "3.50"
---
## Statement 
Each [[Continuity of a Set of Points|continuous]] on a closed finite interval function attains its maximum and minimum, each at least once.
## Proof 
Let $f\in C[a,b]$ ([[Continuity of a Set of Points|Notation]]) be a function. Let us prove that it attains its maximum at some point in $[a,b]$
- Let $(x_n)_{n\in\mathbb N}$ be s [[Sequence]] of points in $[a,b]$ such that $$\lim_{n\to\infty}f(x_n)=\sup f([a,b])$$
- Since $(x_n)_{n\in\mathbb N}$ is a bounded sequence (by $[a,b]$), then it has a converging [[Subsequence]] $(y_n)_{n\in\mathbb N}$
- Since $(y_n)_{n\in\mathbb N}$ is a [[Subsequence]] of $(x_n)_{n\in\mathbb N}: \displaystyle\lim_{n\to\infty}f(y_n)=\lim_{n\to\infty}f(x_n)=\sup f([a,b])$
- Let $y=\displaystyle\lim_{n\to\infty}y_n$; by [[Continuity]] of $f: f(y)=f\left(\displaystyle\lim_{n\to\infty}y_n\right)=\lim_{n\to\infty}f(y_n)=\sup f([a,b])\implies f(y)\max f([a,b]). \blacksquare$ 