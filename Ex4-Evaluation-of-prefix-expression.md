# Ex4 Evaluation of prefix expression
## DATE:25.08.05
## AIM:
To write a java function to evaluate weather the given Matrix A has all odd numbers and Matrix B has all even numbers of the same dimension and find the nature of resultant matrrix.
## Algorithm
1.Start the program.

2.Read the dimensions of both matrices (rows and columns). Check whether Matrix A and Matrix B have the same dimensions. If not, display “Matrices are not of same dimension” and stop.

3.Read Matrix A and check each element: If every element is odd, continue.

4.If any element is even, mark A as invalid and stop further checking.

5.Read Matrix A and check each element: If every element is odd, continue.

6.If any element is even, mark A as invalid and stop further checking.

7.If both matrices are valid, compute the resultant matrix (e.g., A + B or any operation specified). Determine the nature of the resultant matrix:

8.If all elements are odd, print “Resultant matrix is an Odd Matrix”.

9.If all elements are even, print “Resultant matrix is an Even Matrix”. Otherwise, print “Resultant matrix is a Mixed Matrix”.

10.Display the Resultant Matrix.

11.Stop the program. 
  

## Program:
```
/*
Program to evaluate the given prefix expression
import java.util.Scanner;

public class MatrixAddition {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int rows = sc.nextInt();
        int cols = sc.nextInt();

        int[][] A = new int[rows][cols];
        int[][] B = new int[rows][cols];
        int[][] result = new int[rows][cols];

        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                A[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                B[i][j] = sc.nextInt();
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                result[i][j] = A[i][j] + B[i][j];
            }
        }
        for (int i = 0; i < rows; i++) {
            for (int j = 0; j < cols; j++) {
                System.out.print(result[i][j] + " ");
            }
            System.out.println();
        }

       
    }
}

}
Developed by: SANDHIYA SREE B
RegisterNumber: 212223220093 
*/
```

## Output:

<img width="521" height="776" alt="image" src="https://github.com/user-attachments/assets/052842d5-161f-4825-9644-4e8486ba864e" />



## Result:
Thus, the C program to evaluate the prefix expression using stack and print the output of the given prefix expression from the stack inside the function is implemented successfully.
