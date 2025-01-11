import java.util.Scanner;


public class DiagonalElements {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);


        // Input the size of the matrix (it should be a square matrix)
        System.out.print("Enter the size of the square matrix (n x n): ");
        int n = scanner.nextInt();


        // Create the square matrix
        int[][] matrix = new int[n][n];


        // Input elements for the matrix
        System.out.println("Enter elements for the matrix:");
        for (int i = 0; i < n; i++) {
            for (int j = 0; j < n; j++) {
                System.out.print("Matrix[" + i + "][" + j + "]: ");
                matrix[i][j] = scanner.nextInt();
            }
        }


        // Print the main diagonal elements
        System.out.println("\nMain Diagonal Elements:");
        for (int i = 0; i < n; i++) {
            System.out.print(matrix[i][i] + " ");
        }


        // Print the secondary diagonal elements
        System.out.println("\nSecondary Diagonal Elements:");
        for (int i = 0; i < n; i++) {
            System.out.print(matrix[i][n - i - 1] + " ");
        }


        // Close the scanner
        scanner.close();
    }
}


OUTPUT:


Enter the size of the square matrix (n x n): 3
Enter elements for the matrix:
Matrix[0][0]: 1
Matrix[0][1]: 2
Matrix[0][2]: 3
Matrix[1][0]: 4
Matrix[1][1]: 5
Matrix[1][2]: 6
Matrix[2][0]: 7
Matrix[2][1]: 8
Matrix[2][2]: 9


Main Diagonal Elements:
1 5 9 


Secondary Diagonal Elements:
3 5 7










