# 2-by-3-matrix
BBIT-01-0170/2024
Tom Aguko


#include <stdio.h>

#define ROWS 2  // Macro for number of rows
#define COLS 3  // Macro for number of columns

int main() {
    char matrix[ROWS][COLS];

    // Prompt user to enter characters one by one
    printf("Enter values (letters) for a %dx%d matrix:\n", ROWS, COLS);

    for (int i = 0; i < ROWS; i++) {
        for (int j = 0; j < COLS; j++) {
            printf("Enter letter for matrix[%d][%d]: ", i, j);
            scanf(" %c", &matrix[i][j]);  // Space before %c to ignore whitespace
        }
    }

    // Display the entered matrix
    printf("\nThe entered matrix is:\n");
    for (int i = 0; i < ROWS; i++) {
        for (int j = 0; j < COLS; j++) {
            printf("%c\t", matrix[i][j]);
        }
        printf("\n");
    }

    return 0;
}
