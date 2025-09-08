# Which Day

Write a program DayOfWeek.java that takes a date as input and prints the day of the week that date falls on. Your program should take three command-line arguments: m (month), d (day), and y (year). For m use 1 for January, 2 for February, and so forth. For output print 0 for Sunday, 1 for Monday, 2 for Tuesday, and so forth. Use the following formulas, for the Gregorian calendar (where / denotes integer division):

    import java.util.Scanner;
    
    
    public class MyProgram
    {
        public static void main(String[] args)
        {
         Scanner scanner = new Scanner(System.in);
         
         System.out.print("Enter Month(1-12):");
         int m = scanner.nextInt();
         
         if (m > 12) 
            {
                System.out.println("Between 1-12");
                System.exit(0);
            }
         
         System.out.print("Enter Day:");
         int d = scanner.nextInt();
         
         System.out.print("Enter Year:");
         int y = scanner.nextInt();
         
         double y0 = y - (14 - m) / 12;
         double x = y0 + y0 / 4 - y0 / 100 + y0 / 400;
         double m0 = m + 12 * ((14 - m) / 12) - 2;
         double d0 = (d + x + 31*m0 / 12) % 7;
         int result = (int)d0;
    
         System.out.print(result);
        }
    }
