# AIM:
  To write a program to calculate power of a number raised to other using recursion.
 
# ALGORITHM:
  1.
  
  
  
  
  
  
  
  
 # PROGRAM:
   import java.util.Scanner;
   public class Power
   {
      public static void main(String[] args)
      {
        int base , powerRaised;
        Scanner s =new Scanner(System.in);
        System.out.println("Enter the Base value:");
        base=s.nextInt();
        System.out.println("Enter the value of power:");
        powerRaised=s.nextInt();
        int result = power(base, powerRaised);
        System.out.println(base + "^" + powerRaised + "=" + result);
      }
      public static int power(int base, int powerRaised)
      {
        if (powerRaised != 0)
        {
            return (base * power(base, powerRaised - 1));
        }
        else
        {
            return 1;
        }
      }
  }
  
 # OUTPUT:
 
