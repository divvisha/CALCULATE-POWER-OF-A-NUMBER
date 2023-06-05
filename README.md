# EXPERIMENT-6 JAVA PROGRAM TO CALCULATE THE POWER OF A NUMBER USING RECURSION.

# AIM:
  To write a java program to calculate power of a number raised to other using recursion.
 
# ALGORITHM:
  1. Import Scanner to get input for base value and power value from the user.
  2. Using recursion, create a class called power to calculate the output.
  3. If the power value is equal to 0 , then the output will be 1.
  4. If the power is not equal to zero, then the output will be (base * power(base, powerRaised - 1)).
  5. In main class, call the recursion using the class name with arguments.
  6. Print the result.
  
 # PROGRAM:
   import java.util.Scanner;<br>
   public class Power<br>
   {<br>
      public static void main(String[] args)<br>
      {<br>
        int base , powerRaised;<br>
        Scanner s =new Scanner(System.in);<br>
        System.out.println("Enter the Base value:");<br>
        base=s.nextInt();<br>
        System.out.println("Enter the value of power:");<br>
        powerRaised=s.nextInt();<br>
        int result = power(base, powerRaised);<br>
        System.out.println(base + "^" + powerRaised + "=" + result);<br>
      }<br>
      public static int power(int base, int powerRaised)<br>
      {<br>
        if (powerRaised != 0)<br>
        {<br>
            return (base * power(base, powerRaised - 1));<br>
        }<br>
        else<br>
        {<br>
            return 1;<br>
        }<br>
      }<br>
  }
  
 # OUTPUT:
 <img width="243" alt="java ex6 op" src="https://github.com/divvisha/CALCULATE-POWER-OF-A-NUMBER/assets/127508123/ff2c6719-b8ce-494f-a0b4-65d6fa75bdf7">


# RESULT:
  Thus the java program to calculate the power of a number using recursion has been created and executed successfully.
