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

#include <stdio.h> // printf(), scanf()

int main(void) {
	int exam1 = 0, exam2 = 0, exam3 = 0, sum_scores = 0, average = 0;

	// 1: prompt user for exam 1 score
	printf("Enter score 1: ");

	// 2: get score from user
	scanf("%d", &exam1);

	// 3: prompt for exam 2
	printf("Enter score 2: ");

	// 4: get score
	scanf("%d", &exam2);

	printf("Enter score 3: ");
	scanf("%d", &exam3);

	// 5: sum the scores
	sum_scores = exam1 + exam2 + exam3;

	// 6: compute the average
	average = sum_scores / 3;

	// 7: display the average
	printf("Average: %d", average);

	return 0;
}
```

A `#` symbol declares a *preprocessor directive*
- These are examined before compilation