# Ex2 Conversion of the infix expression into postfix expression
## DATE:25.08.25
## AIM:
To write a Java program to Count how many times a number appears in an array recursively.

## Algorithm
1.Read the size of the array and its elements.

2.Read the target number to be counted.

3.Call the recursive function countOccurrences(arr, n, target).

4.In recursion: if size becomes 0, return 0; otherwise check the last element and add 1 if it matches the target.

5.Display the final count returned by the recursive function.

## Program:
```
/*
import java.util.Scanner;

public class CountOccurrences {

    // Recursive function to count occurrences of a target number
    public static int countOccurrences(int[] arr, int n, int target) {
        //write your code here
        if (n == 0) {
            return 0;
        }

        // Check the last element and add 1 if it matches the target
        if (arr[n - 1] == target) {
            return 1 + countOccurrences(arr, n - 1, target);
        } else {
            return countOccurrences(arr, n - 1, target);
        }
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        // Input: Size of array
        int size = scanner.nextInt();

        if (size <= 0) {
            System.out.println("Invalid array size. Must be positive.");
            return;
        }

        // Input: Array elements
        int[] arr = new int[size];
        for (int i = 0; i < size; i++) {
            arr[i] = scanner.nextInt();
        }

        // Input: Target number to count
        int target = scanner.nextInt();

        // Compute and display result
        int count = countOccurrences(arr, size, target);
        System.out.println("The number " + target + " appears " + count + " time(s) in the array.");

        scanner.close();
    }
}



Developed by: SANDHIYA SREE B
RegisterNumber:  212223220093
*/
```

## Output:

<img width="1001" height="632" alt="image" src="https://github.com/user-attachments/assets/2a855062-f7be-4416-bde5-0a16c8f458b5" />


## Result:
Thus, the  program to convert the infix expression into postfix form using stack by following the operator precedence and associative rule is implemented successfully.
