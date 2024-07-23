---
tags:
  - CompArch
---
## Definition
- Two’s complement - the most used notation for signed numbers, which follows these rules:
	- A decimal integer is converted to binary with its sign being ignored
	- “0”s are appended to the left for a required size
	- For positive integers, no more action is needed
	- For negative integers, every bit is inverted and 1 is added
## Example
- $n$ digits cover interval $[-2^{n-1};2^{n-1}-1]$
- $5 = 0101$
- $-5 = 1011$
![[Pasted image 20231004151014.png]]
## Note
- 0 has exactly one representation. 
- It holds the arithmetic property.
- But the reading of a negative pattern is not trivial.