# EX 11 C Program to convert a given decimal value to binary using function without arguments with return type.
## DATE:01/09/2025
## AIM:
To write a C Program to convert a given decimal value to binary using function without arguments with return type.

## Algorithm
1. Start the program.
2. Define a function that reads a decimal number from the user.
3. Convert the number into binary using division by 2 and store remainders.
4. Display the binary value. 
5. Stop the program.  

## Program:
#include <stdio.h>

int decimalToBinary() {
    int num, binary[32], i = 0, j;

    printf("Enter a decimal number: ");
    scanf("%d", &num);

    if (num == 0) {
        printf("Binary: 0\n");
        return 0;
    }

    while (num > 0) {
        binary[i] = num % 2;
        num = num / 2;
        i++;
    }

    printf("Binary: ");
    for (j = i - 1; j >= 0; j--) {
        printf("%d", binary[j]);
    }
    printf("\n");

    return 0;
}

int main() {
    decimalToBinary();
    return 0;
}


## Output:

<img width="1696" height="636" alt="image" src="https://github.com/user-attachments/assets/1335cac5-6807-4aa1-8519-3cd4f9c95835" />


## Result:
Thus the program was executed and the output was verified successfully.
