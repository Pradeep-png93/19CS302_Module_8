## EX NO 8E : HACKERRANK PROBLEM 5
## AIM:
    To write a program to print permutation for the given string.
## ALGORITHM:
 1. Start.
 2. Define a variables.
 3. Write a program to print permutation for the given string.
 4. Read the value using scanf.
 5. Ask the user to make an input.
 6. Print out the answer.
 7. End.
## PROGRAM:
```
#include <stdio.h>
#include <string.h>
void swap(char *x,
char *y) {
 char temp;
 temp = *x;
 *x = *y;
 *y = temp;
}
void permute(char *str,
int l, int r) {
 if (l == r) {
 printf("%s\n", str);
 } else {
 for (int i = l; i <=
r; i++) {
 swap((str + l),
(str + i));
 permute(str, l +
1, r);
 swap((str + l),
(str + i));
 }
 }
}
int main() {
 char str[100];
SAVEETHA ENGINEERING COLLEGE
 printf("Enter a
string: ");
 scanf("%s", str);
 int n = strlen(str);
 printf("All
permutations of the
string are:\n");
 permute(str, 0, n - 1);

 return 0;
}
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/a0ba8932-3544-4066-822b-48b8dd1c26de)


## RESULT:
Thus, the program is executed and verified successfully.

