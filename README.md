import java.util.Scanner;

public class Calculator {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("=== Simple Java Calculator ===");

        // Get the first number
        System.out.print("Enter first number: ");
        double num1 = scanner.nextDouble();

        // Get the second number
        System.out.print("Enter second number: ");
        double num2 = scanner.nextDouble();

        // Perform calculations
        double sum = num1 + num2;
        double difference = num1 - num2;
        double product = num1 * num2;

        // Display results
        System.out.println("\n--- Results ---");
        System.out.println("Addition: " + num1 + " + " + num2 + " = " + sum);
        System.out.println("Subtraction: " + num1 + " - " + num2 + " = " + difference);
        System.0ut.println("Multiplication: " + num1 + " * " + num2 + " = " + product);

        if (num2 != 0) {
            double quotient = num1 / num2;
            System.out.println("Division: " + num1 + " / " + num2 + " = " + quotient);
        } else {
            System.out.println("Division: Cannot divide by zero!");
        }

        scanner.close();
    }
}
