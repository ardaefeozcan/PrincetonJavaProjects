# Triangle Area (Heron)

Area of a triangle. Write a program TriangleArea.java that takes three command line inputs a, b, and c, representing the side lengths of a triangle, and prints the area of the triangle using Heron's formula: area = sqrt(s(s-a)(s-b)(s-c)), where s = (a + b + c) / 2.

    import java.util.Scanner;
    
    public class TriangleArea {
        public static void main(String[] args) {
            Scanner scanner = new Scanner(System.in);
    
            System.out.print("Enter side a: ");
            double a = scanner.nextDouble();
    
            System.out.print("Enter side b: ");
            double b = scanner.nextDouble();
    
            System.out.print("Enter side c: ");
            double c = scanner.nextDouble();
    
            double s = (a + b + c) / 2;
            double area = Math.sqrt(s * (s - a) * (s - b) * (s - c));
    
            System.out.println("Area of triangle: ", area);
        }
    }
