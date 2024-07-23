---
tags:
  - Math
  - Logic
---

## Denotation
- $\Large\frac{Ф_1, Ф_2,...,Ф_n}{\Psi}$
- $Ф_1, Ф_2,...,Ф_n \models \Psi$ 
## Definitions
- $Ф_1, Ф_2,...,Ф_n$ are called *premises*
- $\Psi$ is called *conclusion*
- $(Ф_1\;\&\;Ф_2\;\&\;...\;\&\;Ф_n) \implies \Psi$
## Example
$$\large\frac{a\implies b,\;b\implies c}{a\implies c}$$

| $a$ | $b$ | $c$ | $a\implies b$ | $b\implies c$ | $a\implies c$ |
| --- | --- | --- | ------------- | ------------- | ------------- |
| 0   | 0   | 0   | 1             | 1             | 1             |
| 0   | 0   | 1   | 1             | 1             | 1             |
| 0   | 1   | 0   | 1             | 0             | 1             |
| 0   | 1   | 1   | 1             | 1             | 1             |
| 1   | 0   | 0   | 0             | 1             | 0             |
| 1   | 0   | 1   | 0             | 1             | 1             |
| 1   | 1   | 0   | 1             | 0             | 0             |
| 1   | 1   | 1   | 1             | 1             | 1             |

