#cpt_s_121 

> *Data Type*
> A representation of information and values and the corresponding operations that you can apply

Memory are like storage boxes that allow you to "remember" information for later use

`main.c`
`main`: name of file
`.c`: extension type (to determine compiler used)

```c
/*
 * This is a comment block
 * Name: Neal Wang
 * Date: 2023-08-28
 * Class: CPT_S 121
 * Description: Write a program that prompts the user
 *              for 3 exam scores. Average the 3 scores,
 *              and output to the screen the average
 */

#define _CRT_SECURE_NO_WARNINGS

#include <stdio.h> // printf(), scanf()

int main(void) {
	int exam1 = 0, exam2 = 0, exam3 = 0, sum_scores = 0;
	double average = 0;

	printf("Enter score 1: "); // 1: prompt user for exam 1 score
	scanf("%d", &exam1);	   // 2: get score from user

	printf("Enter score 2: "); // 3: prompt for exam 2
	scanf("%d", &exam2);	   // 4: get score

	printf("Enter score 3: ");
	scanf("%d", &exam3);

	sum_scores = exam1 + exam2 + exam3; // 5: sum the scores
	average = (double)sum_scores / 3;   // 6: compute the average

	printf("Average: %.2lf\n", average); // 7: display the average

	return 0;
}
```

A `#` symbol declares a *preprocessor directive*
- These are examined before compilation

**Integer division**: when dividing integers, the result gets truncated (i.e. 70.8 becomes 70)

## Arithmetic operators

| Operator | Representation | Example |
| -------- | -------------- | ------- |
| + | Addition | 10 + 5 = 15 |
| - | Subtraction | 10.7 - 5.2 = 5.5 |
| * | Multiplication | 2 * 4 = 8 |
| / | Division | 2 / 3 = 0 |
| % | Modulus | 5 % 2 = 1 |

## Printing floating-point numbers

When `printf()`-ing a double `x`, use `printf("%lf", x)`
To round to `n` decimal places, use `printf("%.nlf", x)`

## Type casting

To turn an `int` into a `double`, use `(double)x`