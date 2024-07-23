---
tags:
  - Math
  - AGLA
---
## Definition
- *Ellipse* is a plane curve represented by equation: 
$$\frac{x^2}{a^2}+\frac{y^2}{b^2}=1$$
In some [[Cartesian coordinate system]]

## Vertices 
$$\left(\begin{matrix}\pm a\\0\end{matrix}\right)+\left(\begin{matrix}x_{shift}\\ y_{shift}\end{matrix}\right)$$
$$\left(\begin{matrix}0\\\pm b\end{matrix}\right)+\left(\begin{matrix}x_{shift}\\ y_{shift}\end{matrix}\right)$$
## Foci (a.k.a. focuses)
- Given an ellipse with major axis $2a$. Foci (plural from *focus*) are points $F_1(-c,0), F_2(c,0)$ that satisfy: 
$$c^2=a^2-b^2$$ 
## [[Eccentricity]] 
- Given an ellipse with major axis $2a$ and *foci* $F_1(-c,0),F_2(c,0),$ the eccentricity of ellipse is denoted as 
$$\varepsilon=\frac{c}{a}=\sqrt{1-\frac{b^2}{a^2}},\;0\leq\varepsilon<1$$ 
## Focal Distances
- Distance from a point $M(x,y)$ on an ellipse to each of its *foci*.
	- $r_1=a+x\varepsilon$
	- $r_2=a-x\varepsilon$
- ### Proof $r_1=a+x\varepsilon$ 
	$r_1=\sqrt{(x+c)^2+y^2}\;\&\;$
	$y^2=(a^2-x^2)\frac{b^2}{a^2}\;\&\;$
	$c=a\varepsilon\;\&\;$
	$b^2=a^2-c^2=a^2(1-\varepsilon^2)$
	$\implies y^2=a^2-a^2\varepsilon^2-x^2+x^2\varepsilon^2\implies$ 
	$r_1^2=(x+c)^2+y^2=x^2+2xc+c^2+a^2-a^2\varepsilon^2-x^2+x^2\varepsilon^2=(a+x\varepsilon)^2, \blacksquare$
#### Note that
	$r_2=a-x\varepsilon\implies r_1+r_2=2a$
## [[Latus Rectum]]
- Length = $\displaystyle\frac{2b^2}a$
## Discriminant 
$$D=B^2-4AC<0$$
## Directrices
- *Directrices* are horizontal lines:
	- $x=-\frac{a}{\varepsilon}$
	- $x=\frac{a}{\varepsilon}$
- For given point $M(x,y)$ with $d_1, d_2$ are distances from it to directrices
	- $\frac{r_1}{d_1}=\frac{r_2}{d_2}=\varepsilon$ 
![[Pasted image 20231103155033.png]]
- $d_1=\frac{a}{\varepsilon}+x=\frac{r_1}{\varepsilon}$
## Tangent
$$\frac{x_{tan}x}{a^2}+\frac{y_{tan}y}{b^2}$$
## [[Canonical Equation of an Ellipse]]
## [[General Equation of an Ellipse]]
## [[Parametric Equation of an Ellipse]]
