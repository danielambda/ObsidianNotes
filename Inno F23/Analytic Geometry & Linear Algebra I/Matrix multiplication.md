---
tags:
  - Math
  - AGLA
---
## Definition
$A^{m\times l} * B^{l\times n} = C^{m\times n} \iff \forall i, j: c_{ij} = \displaystyle\sum_{k = 1}^{l} {a_{ik}b_{kj}}$
## Example
$$A = \left[\begin{matrix}a_{11}&a_{12}\\a_{21}&a_{22}\\a_{31}&a_{32}\\a_{41}&a_{42}\end{matrix}\right], B = \left[\begin{matrix}b_{11}&b_{12}&b_{13}\\ b_{21}&b_{22}&b_{23}\end{matrix}\right]$$
$$AB = \left[\begin{matrix}
a_{11}b_{11}+a_{12}b_{21}&a_{11}b_{12}+a_{12}b_{22}&a_{11}b_{13}+a_{12}b_{23}\\ 
a_{21}b_{11}+a_{22}b_{21}&a_{21}b_{12}+a_{22}b_{22}&a_{21}b_{13}+a_{22}b_{23}\\
a_{31}b_{11}+a_{32}b_{21}&a_{31}b_{12}+a_{32}b_{22}&a_{31}b_{13}+a_{32}b_{23}\\
a_{41}b_{11}+a_{42}b_{21}&a_{41}b_{12}+a_{42}b_{22}&a_{41}b_{13}+a_{42}b_{23}\\
\end{matrix}\right]$$
## Properties 
- $AB \not = BA$ (in general)
- $(AB)C = A(BC)$
- $(A + B)C = AC + BC$
- $C(A + B) = CA + CB$