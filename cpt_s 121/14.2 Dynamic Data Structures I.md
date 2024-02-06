---
tags:
  - cpt_s_121
  - pointers
---

-> [Lecture code](https://github.com/mathletedev/cpt_s/blob/main/121/lectures/2023-12-01)

> Uses pointers and dynamically allocated memory.

## `malloc()`

> Allocates memory as needed while a program is running.

```c
#include <stdlib.h>

int *mem_ptr = (int *)malloc(sizeof(int));
```

- Note: `malloc()` returns a `void *`, a **generic pointer**, so cast it with `(int *)`
- Note: `sizeof()` returns the number of bytes needed for a type

Dynamic memory is stored in the **heap**.

**Memory leak**: When memory is allocated but forgotten before it is freed

## Linked lists

```c
typedef struct node {
	int data;
	struct node *next; // self-referential struct, not recursion
} Node;
```