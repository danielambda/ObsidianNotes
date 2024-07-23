---
tags:
  - Algorithms
  - Programming
a.k.a.: LCA
---
## Problem
- Given two strings $X, Y$ we need to find any longest common [[Subsequence]]
## Examples
1. $X=abcbdab, Y=bdcaba$
	- $LCS=bcba$ $X: a\color{aqua}bcb\color{white}d\color{aqua}a\color{white}b, Y:\color{yellow}bd\color{white}ca\color{yellow}ba$
	- $LCS=bdab$ now I'm lazy
## Brute Force Algorithm
1. Try all possible [[Subsequence]]s of $X$: $O(2^{|X|})$
2. Check for each [[Subsequence]] if it is also a [[Subsequence]] of $Y$: $O(2^{|Y|})$
3. Pick the longest one
- Overall complexity: $T(|X|, |Y|)=O(2^{|X|+|Y|})$
## Recursive
- Consider two cases:
	1. $X$ and $Y$ have the same last symbol
		- Then we can always take that symbol
		- $L(n,m)=1+L(n-1,m-1)$
	2. $X$ and $Y$ have different last symbol
		- Then we have to delete last symbol of $X$ or $Y$
		- $L(n,m)=max(L(n,m-1),L(n-1,m))$ 
#### Implementation
```C#
[Pure]
public static int[,] LCS(string X, string Y) 
{
	int n = X.Length;
	int m = Y.Length;
	int[,] L = new int[n+1, m+1];
	
	for (int j = 0; j < n; j++) 
		for (int k = 0; k < m; k++) 
			L[j + 1][k + 1] = 
				X[j] == Y[k] 
				? L[j][k] + 1
				: Math.Max(L[j][k + 1], L[j + 1][k]);

	return L;
}
```