#include <stdio.h>
int recursiveSum(int *n);
int main() {
int number = 10;
int sum;
sum = recursiveSum(&number);
printf("Calculated Sum: %d\n", sum);
return 0;
}
int recursiveSum(int *n) {
int current = *n;
if (current == 0) {
 return 0;
  }
(*n)--;
return current + recursiveSum(n);
}

