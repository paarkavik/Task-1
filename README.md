/*Simple Calulater using Java program*/
//Using Switch Case
import java.util.Scanner;
public class JavaCalculator
{
 public static void main(String[] args)
{
Scanner sc = new Scanner(System.in);
System.out.print("Enter the first number: ");
int Number1 = sc.nextInt();
System.out.print("Enter the second number: ");
int Number2 = sc.nextInt();
System.out.print("Enter the type of operation you want toperform (+, -, *, /, %): ");
String operation = sc.next();
int result = performOperation(Number1, Number2,operation);
System.out.println("Your answer is: " + result);
}
public static int performOperation(int Number1, int Number2, String operation)
{
int result = 0;
switch (operation) {
case "+":
result = Number1 + Number2;
break;
case "-":
result =  Number1 - Number2;
break;
case "*":
result =  Number1 * Number2;
break;
case "%":
result =  Number1 % Number2;
break;
case "/":
result =  Number1 / Number2;
break;
default:
System.out.println(" operation is Invalid");
break;
}
return result;
}
}
