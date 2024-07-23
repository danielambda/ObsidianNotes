---
tags:
  - Programming
---
``` C
struct S {
	int a;
	int b;
};
...
struct S s1;
```
``` C
struct S {
	int a;
	int b;
} s1, s2;
```
``` C
struct {
	int a;
	int b;
} s1, s2, s3;
```
``` C
typedef struct {
	int a;
	int b;
} S;
...
S s1, s2;
```