---
tags:
  - cpt_s_121
---

-> [Lecture code](https://github.com/mathletedev/cpt_s/blob/main/121/lectures/2023-12-08)

```c
#include <stdio.h>

int main(int argc, char *argv[]) {
	for (int i = 0; i < argc; ++i)
		printf("argv[%d]: %s\n", i, argv[i]);

	return 0;
}
```

```bash
./main 1 + 2
```

```
./main
1
+
2
```