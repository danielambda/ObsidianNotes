---
tags:
  - Math
  - MathematicalAnalysis
  - Optimization
---
Seeking a local minima looks like a descent to the lowest point in a [[Neighborhood of real points|neighborhood]]. The best direction to the descent opposites the [[Gradient of the Function]].
## Steps
- Consider an algorithm of the gradient descent. Let $\Delta$ be a length of the step in the opposite of the [[Gradient of the Function]].
	- Define a current point $X$
	- Calculate the [[Gradient of the Function]] $F$ at the current point
	- A step in direction opposite too the gradient: $$Y=X-\Delta\text{grad}(F)$$
	- Check $F(Y)<F(X)$
	- If the condition fulfills then new position $X=Y$
	- Another case a local minimum in the distance less than $\Delta$
## The [[Fastest Gradient-Wise Descent]]