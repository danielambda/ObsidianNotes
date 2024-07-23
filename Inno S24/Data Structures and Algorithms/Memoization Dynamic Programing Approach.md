---
tags:
  - Algorithms
  - Programming
a.k.a.: Top-down
---
## Method
1. Before making a recursive call, check if the result is already know
2. If it is known, use it, otherwise, perform the recursive call 
3. Before exiting the function, save the result in a map or table
## Example 
```
fibonacci(n): 
	initialize empty map F 
	return memo_fib(n, F)
	
memo_fib(n, F):
	if n == 0 then
		return 0
	if n == 1 then
		return 1 
		
	if F.get(n) is null then
		F.put(n, memo_fib(n-1) + memo_fib(n-2))
		
	return F.get(n)
```