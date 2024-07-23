---
tags:
  - Programming
---
## Definition
*Pointer* is an object containing an address to some other object.
```C
int x;
int* p;
...
p = &x;
```
$p$ is a pointer _to_ an int called x
$\&$ is an unary operator "address-of"
``` Pascal
var
p: ponter to int
```

## Types of Pointers
- Pointers to (simple) variables
- Pointers to objects of struct types
- [[Pointers to functions]]:
```C
 int (*pointerToFunction)(long int);
```
Points to a function which takes _long int_ as an argument and returns int
- Pointers to pointers:
```C
int** ptp;
```
- Pointers to values of *any type*
```C
void* anp;
```
## Operators
- $\&$ (unary) -- "address-of"
- $*$ (unary) -- dereferencing: getting object pointed to by a pointer  
- p + integer (binary) -- obvious 
- p - integer (binary) -- is not this the same thing?
- p1 - p2 (binary) -- returns integer of a distance between pointers
## Problem example
``` C
int* p;
void f() {
	int local;
	p = &local;
} 
void main() { 
	f();
	*p = 777; //the hell is gonna happen?
	//actually nothing specific
}
```