---
tags:
  - Algorithms
  - Programming
a.k.a.: Bottom-up approach
---
## Method
1. Initialize a table that will contain solutions to all subproblems
2. Fill in the table, starting from the smallest subproblems
3. Extract the solution to the original problem from the table
## Example
```
fibonacci(n): 
	initialize array F of size n+1
	f[0] = 0
	f[1] = 1
	for i from 2 to n
		f[i] = f[i-1] + f[i-2]
	return f[n]
```