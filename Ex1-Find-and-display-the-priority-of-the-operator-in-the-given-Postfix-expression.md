# EX 1 Display operator precedence in the infix expression.
## DATE:25.08.05
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## Algorithm
1.Start the program.

2.Input the infix expression 

3.Extract each character one by one from the expression.

4.Check if the symbol is an operator 

5.If it is not an operator (like numbers), skip it.


6.Use a switch-case statement to check which operator it is.

7.For each operator, return a numeric value representing its precedence.

8.Back in main(), after receiving the priority value,

9.Match the numeric value to the meaning of priority (e.g., “Lowest Priority”, “Second Highest Priority”).

1.0Display the operator and its priority meaning.

11.Repeat the steps until all operators in the expression are processed.

12.End the program. 

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
import java.util.*;

public class Main {
    static int getMin(int[] arr, int i, int n) {
        if (i == n - 1) {
            return arr[i];
        }

    
        int minRest = getMin(arr, i + 1, n);
       
        return Math.min(arr[i], minRest);
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        int[] arr = new int[n];
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }
        System.out.println(getMin(arr, 0, n));
    }
}
   
Developed by: SANDHIYA SREE B
RegisterNumber:  212223220093
*/
```

## Output:

<img width="641" height="296" alt="image" src="https://github.com/user-attachments/assets/939b96d1-f704-4d36-945f-ead6d622f433" />



## Result:
Thus the C program to find and display the priority of the operator in the given Postfix expression is implemented successfully
