# Body Mass Index (BMI)

Body mass index. The body mass index (BMI) is the ratio of the weight of a person (in kilograms) to the square of the height (in meters). Write a program BMI.java that takes two command-line arguments, weight and height, and prints the BMI.

    import java.util.Scanner;
    
    public class BMI {
        public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);
    
            System.out.print("Enter weight (kg): ");
            double weight = scanner.nextDouble();
    
            System.out.print("Enter height (m): ");
            double height = scanner.nextDouble();
    
            double bmi = weight / (height * height);
            System.out.println("BMI: ", bmi);
        }
    }
