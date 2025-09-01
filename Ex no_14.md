# EX 14 C program to delete first element in an array.
## DATE:01/09/2025
## AIM:
To write a C program to delete first element in an array.

## Algorithm
1. Start the program.
2. Read the size of the array and its elements from the user.
3. To delete the first element, shift each element of the array one position to the left.
4. Reduce the effective size of the array by one. 
5. Print the updated array.  

## Program:
#include <stdio.h>

int main() {
    int arr[50], n, i;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Shift elements to delete the first element
    for (i = 0; i < n - 1; i++) {
        arr[i] = arr[i + 1];
    }
    n--; // Reduce array size

    printf("Array after deleting the first element:\n");
    for (i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");

    return 0;
}


## Output:

<img width="1771" height="650" alt="image" src="https://github.com/user-attachments/assets/efe9431e-7440-4153-8cc4-cc1314c8454f" />


## Result:
Thus the program was executed and the output was verified successfully.
