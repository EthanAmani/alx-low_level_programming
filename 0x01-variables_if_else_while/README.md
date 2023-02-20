#include <stdio.h>
#include <stdlib.h>
#include <time.h>

/**
 * main - generates a random number and prints whether it's positive or negative
 *
 * Return: always 0
 */
int main(void)
{
	srand(time(NULL));
	int n = rand() - RAND_MAX / 2;

	printf("%d ", n);
	if (n > 0)
		printf("is positive\n");
	else if (n == 0)
		printf("is zero\n");
	else
		printf("is negative\n");

	return (0);
}

