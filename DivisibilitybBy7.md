# Divisibility by 7

Write a program Divisibility.java that reads in two command line inputs and prints true if both are divisible by 7, and false otherwise.

    import java.util.Scanner;
    
    public class Divisibility {
        public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);
    
            System.out.print("Enter first number: ");
            int a = scanner.nextInt();
    
            System.out.print("Enter second number: ");
            int b = scanner.nextInt();
    
            boolean bothDivisible = (a % 7 == 0) && (b % 7 == 0);
            System.out.println(bothDivisible);
        }
    }
