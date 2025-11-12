# EX 1 You’re creating a health monitoring device which stores several sensor readings in an array. To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
## DATE:12/11/2025
## AIM:
To write a JAVA program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.

## Algorithm
```
1.Start the program.
2.Read the array elements.
3.Define a recursive function findMin(arr, n):
4.Base case: If array size is 1, return the element.
5.Recursive case: Return the smaller value between arr[n-1] and findMin(arr, n-1).
6.Display the result.
7.Stop the program.
```

## Program:
```
/*
Program To determine the minimum value (e.g., lowest heartbeat), implement a recursive method.
Developed by: Reshma R
RegisterNumber:  212224040274
*/
```
```
import java.util.*;

public class MinValueRecursion {
    static int findMin(int[] arr, int n) {
        if (n == 1)
            return arr[0];
        return Math.min(arr[n - 1], findMin(arr, n - 1));
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter number of readings: ");
        int n = sc.nextInt();
        int[] arr = new int[n];
        System.out.println("Enter the readings:");
        for (int i = 0; i < n; i++)
            arr[i] = sc.nextInt();

        int minValue = findMin(arr, n);
        System.out.println("Lowest heartbeat (Minimum Value): " + minValue);
    }
}
```

## Output:
<img width="1915" height="774" alt="image" src="https://github.com/user-attachments/assets/d534802a-1301-45f6-b283-b5d84d8fc5b1" />



## Result:
Thus the JAVA prograM ti find the minimum value (e.g., lowest heartbeat), implement a recursive method has implemented successfully
