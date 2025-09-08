# Three-sort

Three-sort. Write a program ThreeSort.java that takes three int values from the command line and prints them in ascending order. Use Math.min() and Math.max().

    import java.util.Scanner;
    
    public class MyProgram
    {
        public static void main(String[] args)
        {
            Scanner scanner = new Scanner(System.in);
            
            System.out.print("Number 1:");
            int num1 = scanner.nextInt();
            System.out.print("Number 2:");
            int num2 = scanner.nextInt();
            System.out.print("Number 3:");
            int num3 = scanner.nextInt();
            
            int min = Math.min(num1, Math.min(num2, num3));
            int max = Math.max(num1, Math.max(num2, num3));
            int middle = num1 + num2 + num3 - min - max;
    
            System.out.println(min + " " + middle + " " + max);
            
        }
    }
