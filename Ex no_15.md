# EX 15 C program that reads a one-dimensional array of integers and replaces all even elements with 'E'.
## DATE:01/09/2025
## AIM:
To write a C program that reads a one-dimensional array of integers and replaces all even elements with 'E'.

## Algorithm
1. Start the program.
2. Read the size of the array and its elements from the user.
3. Traverse the array using a loop.
4. If an element is even, replace it with 'E'. 
5. Print the updated array.  

## Program:
#include <stdio.h>

int main() {
    int n, i;
    int arr[50];

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter %d integers:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("Array after replacing even elements with 'E':\n");
    for (i = 0; i < n; i++) {
        if (arr[i] % 2 == 0)
            printf("E ");
        else
            printf("%d ", arr[i]);
    }
    printf("\n");

    return 0;
}


## Output:

<img width="1603" height="674" alt="image" src="https://github.com/user-attachments/assets/50f94157-f83e-46cf-b08b-3ae16ded6bb7" />


## Result:
Thus the program was executed and the output was verified successfully.
