# Ex5 Stack Operations
## DATE:25.08.25
## AIM:To write a Java program to Count the number of inversions in an array where inversion is defined as: arr[i] > arr[j] and i < j
## Algorithm
1.Start the program.

2.Read the number of elements and store them in an array.

3.Use a modified merge sort to count inversions: .Recursively split the array into halves and count inversions in each half. .While merging two sorted halves,

4.count cross inversions when an element from the right half is placed before elements remaining in the left half.

5.Sum inversions from left half, right half, and cross inversions.

6.Display the total inversion count.

7.Stop the program.
## Program:
```
/*
import java.util.Scanner;

public class CountInversions {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int n = sc.nextInt();
        int[] arr = new int[n];

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        long result = mergeSortAndCount(arr, 0, n - 1);
        System.out.println(result);
    }

    private static long mergeSortAndCount(int[] arr, int left, int right) {
        long count = 0;
        if (left < right) {
            int mid = (left + right) / 2;
            count += mergeSortAndCount(arr, left, mid);
            count += mergeSortAndCount(arr, mid + 1, right);
            count += mergeAndCount(arr, left, mid, right);
        }
        return count;
    }

    private static long mergeAndCount(int[] arr, int left, int mid, int right) {
        int[] leftArr = new int[mid - left + 1];
        int[] rightArr = new int[right - mid];

        System.arraycopy(arr, left, leftArr, 0, leftArr.length);
        System.arraycopy(arr, mid + 1, rightArr, 0, rightArr.length);

        int i = 0, j = 0, k = left;
        long swaps = 0;

        while (i < leftArr.length && j < rightArr.length) {
            if (leftArr[i] <= rightArr[j]) {
                arr[k++] = leftArr[i++];
            } else {
                arr[k++] = rightArr[j++];
                swaps += (mid + 1) - (left + i);
            }
        }

        while (i < leftArr.length) {
            arr[k++] = leftArr[i++];
        }
        while (j < rightArr.length) {
            arr[k++] = rightArr[j++];
        }

        return swaps;
    }
}

Developed by: SANDHIYA SREE B
RegisterNumber:  212223220093
*/
```

## Output:
<img width="822" height="227" alt="image" src="https://github.com/user-attachments/assets/e17d6d7f-fd7a-4b39-b47b-ff6439f1c421" />



## Result:
Thus the  program to perform push and pop operation of the stack in the infix to postfix conversion is implemented successfully.
