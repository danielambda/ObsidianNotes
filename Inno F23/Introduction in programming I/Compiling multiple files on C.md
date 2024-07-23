---
tags:
  - Programming
---

Firstly you have to compile each \*.c file into a \*.o file and only after that you are allowed to compile all of the \*.o files into an executable.

#### Example:
```
gcc -c foo.c 
gcc -c main.c
gcc -c bar.c
gcc -o fubar foo.o main.o bar.o -lm
```

#### Details: 
-lm means link using math library 
