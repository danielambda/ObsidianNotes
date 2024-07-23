---
tags:
  - CompArch
  - Math
---
## Definition
- It is a version of arithmetic in which all operations such as addition and multiplication are limited to a fixed range between a minimum and maximum value. 
- If the result of an operation is greater than the maximum, it is clamped to the maximum. 
- If it is below the minimum, it is clamped to the minimum
## Example
- Valid range is $[-100;100]$:
	- $60+30 = 90$
	- $60+43 = 100$
	- $(60+43) - (75+75) = 0$
	- $99\times99=100$
## Advantages
- Saturation arithmetic enables efficient algorithms for many problems, particularly in digital signal processing. 
- For example: 
	- Adjusting the volume level of a sound signal can result in overflow, and saturation causes significantly less distortion to the sound than wrap-around.