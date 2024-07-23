---
tags:
  - CompArch
---
## Definition
- The leftmost bit defines the sign of the number (0 for +; 1 for -) 
- The integer is changed to binary (the sign is ignored)
- 0s are added to the left of the number to make a total of N bits 
- If the sign is positive, no more action is needed. If the sign is negative, every bit is inverted Represented interval: $[-2n−1 +1, 2n−1 -1]$ 
- Note: The name ”ones’ complement” refers to the fact that such an inverted value, if added to the original, would always produce an ’all ones’ number
## Example
- 4 digits represent interval $[-7;7]$
- $5 = 0101$
- $-5 = 1010$ unlike $1101$ for [[Sign and Magnitude Representation]]
![[Pasted image 20231004150654.png]]
## Issues
- A negative number is represented by flipping all the bits of a positive number.
- Still have two patterns for $0$