# Power-of-a-Number-using-Recursion-in-Java

Power of a Number using Recursion in Java
Here, in this page we will discuss the program to find power of a number using recursion in java programming language. We are given with two integers values base and power respectively. We need to print the value representing the base raise to its power. We will design the program using recursion and also discuss the approach using iteration as well.

Example :

Input : 5 3
Output : 125
Explanation : 53 = 125
Power of a Number using Recursion in Java
Method 1 (Using Recursion):
Create a recursive function say power(int base, int x)
Base condition : if(x==0) return 1.
Otherwise, return (base* power(base, x-1))
Power of a number
Time and Space Complexity
Time Complexity : O(x), x denotes the power. Space Complexity : O(1)
Java Code
Run
public class Main
{
  public static void main (String[]args)
  {
    int base = 5, x = 3;
    System.out.println ("Required Power is " + power (base, x));
  }
  //Recursive Function
  static int power (int base, int x)
  {
    if (x == 0)     //Base Condition
      return 1;
    return (base * power (base, x - 1));
  }
}
Output
Required Power is 125
Related Pages
Finding Number of times x digit occurs in a given input
 
Finding number of integers which has exactly x divisors
 
Smallest element in an array

Prime Number

Largest element in an array

Method 2 (Using Loop):
Create a function say power(int base, int x), that will return the integer value denoting the basex.
Create a variable say result = 1, that hold the basex.
Run a while loop that will terminate when x becomes 0.
Inside the loop set result = result * base.
After complete iteration return result.
Time and Space Complexity
Time Complexity : O(x), x denotes the power. Space Complexity : O(1)
Run
class Main {
    public static void main(String[] args) {
        int base = 5, x = 3;
        System.out.println("Required Power is " + power(base, x));
    }
    static int power(int base, int x) {
        int result = 1;
        while (x > 0) {
            result *= base;
            x--;
        }
        return result;
    }
}
Output
Required Power is 125
