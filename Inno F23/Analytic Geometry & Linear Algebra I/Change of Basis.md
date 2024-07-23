---
tags:
  - Math
  - AGLA
---
## [[Cartesian coordinate system]]
## Action itself
- Old coordinate system: $0, \overline e_1, \overline e_2, \overline e_3$
- New coordinate system: $0', \overline e_1', \overline e_2', \overline e_3'$
![[Changing the Basisi.excalidraw]]
- $\overline e_1'= \alpha_{11}\overline e_1 + \alpha_{21}\overline e_2 + \alpha_{31}\overline e_3$ 
- $\overline e_2'= \alpha_{12}\overline e_1 + \alpha_{22}\overline e_2 + \alpha_{32}\overline e_3$ 
- $\overline e_3'= \alpha_{13}\overline e_1 + \alpha_{23}\overline e_2 + \alpha_{33}\overline e_3$ 
- $\overline{00'} = \beta_1\overline e_1 + \beta_2\overline e_2 +\beta_3\overline e_3$
---
Expressing the point $M$ 
### Theorem:
- $M(x_1, x_2, x_3)$ - old 
- $M(x_1', x_2', x_3')$ - new
	- $x_1 = \alpha_{11} x_1' + \alpha_{12} x_2' +  \alpha_{13} x_3' + \beta_1$
	- $x_2 = \alpha_{21} x_1' + \alpha_{22} x_2' +  \alpha_{33} x_3' + \beta_2$
	- $x_3 = \alpha_{11} x_1' + \alpha_{12} x_2' +  \alpha_{13} x_3' + \beta_3$
### Proof:
- $\overline {OM} = \overline {O'M} + \overline {OO'}$
- $x_1\overline e_1 + x_2\overline e_2 + x_3\overline e_3 =$ 
$= x_1'\overline e_1' + x_2'\overline e_2' + x_3'\overline e_3' + \overline{OO'} =$
$= x_1'(\alpha_{11}\overline e_1 + \alpha_{21}\overline e_2 + \alpha_{31}\overline e_3) +$  
$+ x_2'(\alpha_{12}\overline e_1 + \alpha_{22}\overline e_2 + \alpha_{32}\overline e_3) +$
$+ x_3'(\alpha_{13}\overline e_1 + \alpha_{23}\overline e_2 + \alpha_{33}\overline e_3) +$
$+ \beta_1\overline e_1 + \beta_2\overline e_2 +\beta_3\overline e_3 =$
$= \overline e_1(x_1'\alpha_{11} + x_2'\alpha_{12} + x_3'\alpha_{13} + \beta_1) +$
$+ \overline e_2(x_1'\alpha_{21} + x_2'\alpha_{22} + x_3'\alpha_{23} + \beta_2) +$
$+ \overline e_3(x_1'\alpha_{31} + x_2'\alpha_{32} + x_3'\alpha_{33} + \beta_3)\implies$
$$\implies\begin{matrix}x_1 = x_1'\alpha_{11} + x_2'\alpha_{12} + x_3'\alpha_{13} + \beta_1\\ x_2 = \alpha_{21} x_1' + \alpha_{22} x_2' +  \alpha_{33} x_3' + \beta_2 \\ x_3 = \alpha_{11} x_1' + \alpha_{12} x_2' +  \alpha_{13} x_3' + \beta_3\end{matrix}$$
### [[Matrix|Matrix]] representation 

$$\left[\begin{matrix}x_1\\ x_2 \\ x_3\end{matrix}\right] = A\left[\begin{matrix}x_1'\\ x_2' \\ x_3'\end{matrix}\right] + \overline{OO'} = \left[\begin{matrix}\alpha_{11}&\alpha_{12}&\alpha_{13}\\ \alpha_{21}&\alpha_{22}&\alpha_{23}\\ \alpha_{31}&\alpha_{32}&\alpha_{33}\end{matrix}\right]\left[\begin{matrix}x_1'\\ x_2' \\ x_3'\end{matrix}\right] + \overline{OO'}$$
## [[Rotating a plane]]