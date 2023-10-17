//# Addition-of-Matrix
#include <stdio.h>

int main() {
  int row, col;
  int mat1[row][col], mat2[row][col], res[row][col];

  // Read the number of rows and columns
  printf("Enter the number of rows and columns: ");
  scanf("%d %d", &row, &col);

  // Read the first matrix
  printf("Enter the elements of the first matrix: ");
  for (int i = 0; i < row; i++) {
    for (int j = 0; j < col; j++) {
      scanf("%d", &mat1[i][j]);
    }
  }

  // Read the second matrix
  printf("Enter the elements of the second matrix: ");
  for (int i = 0; i < row; i++) {
    for (int j = 0; j < col; j++) {
      scanf("%d", &mat2[i][j]);
    }
  }

  // Add the two matrices
  for (int i = 0; i < row; i++) {
    for (int j = 0; j < col; j++) {
      res[i][j] = mat1[i][j] + mat2[i][j];
    }
  }

  // Print the result
  printf("The result of adding the two matrices is: \n");
  for (int i = 0; i < row; i++) {
    for (int j = 0; j < col; j++) {
      printf("%d ", res[i][j]);
    }
    printf("\n");
  }

  return 0;
}
