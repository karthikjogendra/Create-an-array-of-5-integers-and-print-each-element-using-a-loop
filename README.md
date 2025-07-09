# Create-an-array-of-5-integers-and-print-each-element-using-a-loop
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        int[] arr = new int[5]; // Array of 5 integers
        Scanner sc = new Scanner(System.in);

        System.out.println("Enter 5 integers:");
        for (int i = 0; i < 5; i++) {
            arr[i] = sc.nextInt(); // Input values
        }

        System.out.println("Array elements are:");
        for (int i = 0; i < 5; i++) {
            System.out.print(arr[i] + " "); // Print values
        }
        System.out.println();

        int maxVal = arr[0]; // Assume first element is max
        for (int i = 1; i < 5; i++) {
            if (arr[i] > maxVal) {
                maxVal = arr[i]; // Update if current is greater
            }
        }

        System.out.println("Maximum element is: " + maxVal);
    }
}
