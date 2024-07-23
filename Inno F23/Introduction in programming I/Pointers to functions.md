---
tags:
  - Programming
---
## Example
``` C
char f(int p)
{
	...
}
...
char (*pf)(int) = &f;
...
void main()
{
	char ch1 = f(1);
	char ch2 = pf(1); 
	return 0;
}
```