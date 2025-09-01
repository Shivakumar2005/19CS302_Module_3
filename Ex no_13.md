read the elements and print only the odd elements in the 2D array.
## DATE:01/09/2025
## AIM:
To write a C program to read the elements and print only the odd elements in the 2D array.

## Algorithm
1. Start the program.
2. Declare a 2D array and variables for rows and columns.
3. Read the number of rows and columns from the user.
4. Input all elements into the 2D array. 
5. Traverse the array and print only the odd elements.  

## Program:
#include <stdio.h>

int main() {
    int rows, cols, i, j;

    printf("Enter number of rows: ");
    scanf("%d", &rows);
    printf("Enter number of columns: ");
    scanf("%d", &cols);

    int arr[rows][cols];

    printf("Enter the elements of the 2D array:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            scanf("%d", &arr[i][j]);
        }
    }

    printf("Odd elements in the 2D array are:\n");
    for (i = 0; i < rows; i++) {
        for (j = 0; j < cols; j++) {
            if (arr[i][j] % 2 != 0) {
                printf("%d ", arr[i][j]);
            }
        }
    }
    printf("\n");

    return 0;
}


## Output:

<img width="1771" height="630" alt="image" src="https://github.com/user-attachments/assets/0319ec46-f54c-4081-b1f9-f06a1a62eccc" />


## Result:
Thus the program was executed and the output was verified successfully.
