---
tags:
  - CompArch
---
## Transformation of  [[Set Reset Latch]] into a Flip-Flop
![[Pasted image 20231019153257.png]]
Step 1:
	Inclusion of a clock generator
Step 2:
	Adding "AND" gates to propagate "S" and "R" at asserted clock states only
Step 3:
	Adding another "slave" latch with 2 "AND" gates
Step 4:
	Providing Q to "slave"
Step 5:
	Providing inverted clock signal to "slave"
![[Pasted image 20231019154016.png]]
