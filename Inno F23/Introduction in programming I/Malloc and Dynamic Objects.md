---
tags:
  - Programming
---
## Definition
- **Dynamic objects** are the ones that are created at any moment during program execution. The lifetime of dynamic objects is not under the scoping rules.
- **malloc** (shortcut for memory allocation) is a special library function that allocates $n$ bytes in memory and returns \*void pointer 
## Example
``` C
void* p = malloc(8);
int* pi = (int*)malloc(4);
```
## Important
\*void pointers can be converted to any pointer type
## Formal definition for adding integers to pointers
``` C
T* p;
...p + i; <=> ...(T*)((char*)p + sizeof(T) * i);
```
