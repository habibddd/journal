### do-while
> The `do-while` loop is a structure that allows to perform an action once and then have it repeat as long as a specified condition evaluates to true.
> This is particularly helpful when you want the loop body to execute at least once (for example asking for user input and validating it).
```
do {
action that runs once and keeps repeating
} while (this condition is true);
```

```c
#include <stdio.h>

int main(void) {
  int n = 0;
  
  do {
    printf("This action will run once and then repeat as long as the while condition is true, so until n reaches %d.\n", n);
    n ++;
  } while (n < 5);
  
  printf("This is the value of n after the loop has been stopped: %d\n", n);
  
  return 0;
}
```
```
Output:
This action will run once and then repeat as long as the while condition is true, so until n reaches 0.
This action will run once and then repeat as long as the while condition is true, so until n reaches 1.
This action will run once and then repeat as long as the while condition is true, so until n reaches 2.
This action will run once and then repeat as long as the while condition is true, so until n reaches 3.
This action will run once and then repeat as long as the while condition is true, so until n reaches 4.
This is the value of n after the loop has been stopped: 5.
```
>[!TIP]
>If the variable compound assignment had been placed before the first `printf` the "count" would have started from `1` instead of `0`.
>The final value of n doesn't change because that is ruled by the while condition `n < 5`:
```c
#include <stdio.h>

int main(void) {
  int n = 0;
  
  do {
    n ++;
    printf("This action will run once and then repeat as long as the while condition is true, so until n reaches %d.\n", n);
  } while (n < 5);
  
  printf("This is the value of n after the loop has been stopped: %d\n", n);
  
  return 0;
}
```
```
Output:
This action will run once and then repeat as long as the while condition is true, so until n reaches 1.
This action will run once and then repeat as long as the while condition is true, so until n reaches 2.
This action will run once and then repeat as long as the while condition is true, so until n reaches 3.
This action will run once and then repeat as long as the while condition is true, so until n reaches 4.
This action will run once and then repeat as long as the while condition is true, so until n reaches 5.
This is the value of n after the loop has been stopped: 5.
```
