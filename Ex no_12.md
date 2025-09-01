# EX 12 C program to check whether the given number is prime or not using function without return type and with arguments.
## DATE:01/09/2025
## AIM:
To write a C program to check whether the given number is prime or not using function without return type and with arguments.

## Algorithm
1. Start the program.
2. Define a function that takes an integer argument.
3. In the function, check if the number is divisible by any integer from 2 to n/2.
4.  If divisible, print that it is not prime; otherwise, print that it is prime.
5.  Stop the program. 

## Program:
#include <stdio.h>

void checkPrime(int n) {
    int i, flag = 0;

    if (n <= 1) {
        printf("%d is not a prime number.\n", n);
        return;
    }

    for (i = 2; i <= n / 2; i++) {
        if (n % i == 0) {
            flag = 1;
            break;
        }
    }

    if (flag == 0)
        printf("%d is a prime number.\n", n);
    else
        printf("%d is not a prime number.\n", n);
}

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);

    checkPrime(num);

    return 0;
}


## Output:

<img width="1405" height="686" alt="image" src="https://github.com/user-attachments/assets/4e97be61-fbb2-40d5-a65d-811570fa3341" />


## Result:
Thus the program was executed and the output was verified successfully.
