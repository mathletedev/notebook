#cpt_s_121

> A sequence of instructions that solve a problem

- A well ordered collection...
- Of unambiguous and effectively computable operations...
- That produces a result...
- And halts in a finite amount of time.

## Types of instructions

- Sequenced instructions
	- do them in the order given
- Conditional instructions
	- do them if a condition is true
- Iterative instructions
	- do them while a condition is true

```c
/*
* Name: Neal Wang
* Date: 2023-08-25
* Class: CPT_S 121
* Lab section: 08
* Description: Output to the screen a message that says
*              "Hello, CPT_S 121!"
*/

#include <stdio.h> // contains utility functions to output text to screen - printf()

int main(void) { // starting point of execution for every C program
	printf("Hello, CPT_S 121!");

	return 0;
}
```