---
tags:
  - Math
  - MathematicalAnalysis
  - DifferetialForms
  - ExteriorAlgebra
---
## Definition
- For [[Differential m-Form]] $\omega$ on $\mathbb R^n$
$$d\omega=\sum_I\sum_{j=1}^n\frac{\partial f}{\partial x_j}dx_j\wedge dx_I$$
## Properties
#### [[Linearity]]
#### $d^2=0$
##### Proof
$$d^2\omega=d(d\omega)=d\left(\sum_I\sum_{j=1}^n\frac{\partial f}{\partial x_j}dx_j\wedge dx_I\right)=\sum_I\sum_{k=1}^n\sum_{j=1}^n\frac{\partial^2f}{\partial x_k x_j}dx_k\wedge dx_j\wedge dx_I=$$
$$=\sum_I\sum_{k=1}^n\left(\sum_{j=1}^{k-1}\frac{\partial^2f}{\partial x_k x_j}dx_k\wedge dx_j\wedge dx_I+0+\sum_{j=k+1}^{n}\frac{\partial^2f}{\partial x_k x_j}dx_k\wedge dx_j\wedge dx_I\right)=$$
$$=\sum_I\left(\sum_{k=1}^n\sum_{j=1}^{k-1}\frac{\partial^2f}{\partial x_k x_j}dx_k\wedge dx_j\wedge dx_I+\sum_{j=1}^{n}\sum_{k=1}^{j-1}\frac{\partial^2f}{\partial x_k x_j}dx_k\wedge dx_j\wedge dx_I\right)=$$
$$=\sum_I\left(\sum_{k=1}^n\sum_{j=1}^{k-1}\frac{\partial^2f}{\partial x_k x_j}dx_k\wedge dx_j\wedge dx_I\color{red}-\color{white}\sum_{j=1}^{n}\sum_{k=1}^{j-1}\frac{\partial^2f}{\color{red}\partial x_j x_k}\color{red}dx_j\wedge dx_k\color{white}\wedge dx_I\right)=\sum_I0=$$$$\Large= 0\;\blacksquare$$
#### $\omega$ =[[Differential m-Form|Differential k-Form]], $\mu$ = [[Differential m-Form|Differential m-Form]]
$$d(\omega\wedge\mu)=(d\omega)\wedge\mu+(-1)^k\omega\wedge(d\mu)$$
##### Proof
$$\omega=\sum_I f_I dx_I,\mu=\sum_J g_J dx_J$$
$$\omega\wedge\mu=\sum_{I,J} f_I g_J\;dx_I\wedge dx_J$$
$$d(\omega\wedge\mu)
=\sum_{I,J}\sum_{r=1}^{k+m} \frac{\partial f_I g_J}{\partial x_r}\;dx_r\wedge dx_I\wedge dx_J=$$
$$=\sum_{I,J}\sum_{r=1}^{k+m} \left(\frac{\partial f_I}{\partial x_r}\times g_J+f_I\times\frac{\partial g_j}{\partial x_r}\right)\;dx_r\wedge dx_I\wedge dx_J=$$
$$=\sum_{I,J}\sum_{r=1}^{k+m} \frac{\partial f_I}{\partial x_r}\times g_J\;dx_r\wedge dx_I\wedge dx_J+\sum_{I,J}\sum_{r=1}^{k+m} f_I\times\frac{\partial g_j}{\partial x_r}\;dx_r\wedge dx_I\wedge dx_J=$$
$$=\sum_{I,J}\sum_{r=1}^{k+m} \frac{\partial f_I}{\partial x_r}\times g_J\;dx_r\wedge dx_I\wedge dx_J\color{red}+(-1)^{k}\color{white}\sum_{I,J}\sum_{r=1}^{k+m} f_I\times\frac{\partial g_j}{\partial x_r}\;\color{red}dx_I\wedge dx_r\color{white}\wedge dx_J=$$
$$(d\omega)\wedge \mu+(-1)^k\omega\wedge(d\mu)\;\blacksquare$$
see [[Arithmetic operations with Derivatives]]
## Notation
- Exterior derivative is written using $d$ operator. Exterior derivative for [[Differential m-Form]] $\omega$ is $d\omega$
## Note that
$$d(fd_I)=\frac{\partial f}{\partial x_1}dx_1\wedge dx_I+...+\frac{\partial f}{\partial x_n}dx_n\wedge dx_I$$