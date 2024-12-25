package unit;

import java.util.Scanner;

public class New {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("--- BMI Calculator ---");

        // Input weight
        System.out.print("Enter your weight in kilograms (kg): ");
        double weight = scanner.nextDouble();

        // Input height
        System.out.print("Enter your height in meters (m): ");
        double height = scanner.nextDouble();

        // Calculate BMI
        double bmi = calculateBMI(weight, height);

        // Display BMI result
        System.out.printf("Your BMI is: %.2f%n", bmi);

        // Display BMI category
        String category = classifyBMI(bmi);
        System.out.println("You are classified as: " + category);
    }

    // Method to calculate BMI
    public static double calculateBMI(double weight, double height) {
        return weight / (height * height);
    }

    // Method to classify BMI
    public static String classifyBMI(double bmi) {
        if (bmi < 18.5) {
            return "Underweight";
        } else if (bmi >= 18.5 && bmi < 24.9) {
            return "Normal weight";
        } else if (bmi >= 25 && bmi < 29.9) {
            return "Overweight";
        } else {
            return "Obesity";
        }
    }
}
