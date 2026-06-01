# 19AI304 - Fundamentals of C Programming - Even Junior -2026

# IAPR 1 - Module 1

# Exp.1 : Check Even or Odd Using Pointer

## Aim:

To determine whether a number entered by the user is even or odd using a pointer.

## Algorithm:

1. Start the program.
2. Declare an integer variable n and a pointer p.
3. Read the number from the user and store it in n.
4. Assign the address of n to the pointer p.
5. Check the value pointed by p:
   * If divisible by 2 → the number is even.
   * Otherwise → the number is odd.
6. Print the result.
7. End the program.

## Program:

```c
#include <stdio.h>

int main()
{
    int n;
    scanf("%d", &n);
    int *p;
    p = &n;

    if (*p % 2 == 0) {
        printf("%d is even.", *p);
    } else {
        printf("%d is odd.", *p);
    }

    return 0;
}
```

## Output:

<img width="459" height="164" alt="502993474-4d2aa4b3-a0ad-4dc2-8e83-17865061ce43" src="https://github.com/user-attachments/assets/1ee9512f-9b40-48e9-b472-7c90023c4dc4" />

## Result:

Thus, The C program to determine whether a number entered by the user is even or odd using a pointer was successfully executed.

***

# Exp.2 : Sum of Digits Using Recursion

## Aim:

To write a C program that calculates the sum of digits of a given number using recursion.

## Algorithm:

1. Start the program.
2. Define a recursive function sumOfDigits(int n) that:
   * Returns 0 if n is 0 (base case).
   * Otherwise, returns (n % 10) + sumOfDigits(n / 10) to sum the last digit with the recursive call for the remaining digits.
3. In the main() function:
   * Read an integer n from the user.
   * Call the recursive function sumOfDigits(n) and store the result.
   * Print the sum of digits.
4. End the program.
