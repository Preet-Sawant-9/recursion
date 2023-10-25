Recursion
THEORY
Recursion is the technique of making a function call itself. This technique provides a way to break complicated problems down into simple problems which are easier to solve.

Recursion may be a bit difficult to understand. The best way to figure out how it works is to experiment with it.

Recursion Example Adding two numbers together is easy to do, but adding a range of numbers is more complicated. In the following example, recursion is used to add a range of numbers together by breaking it down into the simple task of adding two numbers:

Example

int sum(int k)

{

if (k > 0)

{

return k + sum(k - 1);
}

else

{

return 0;
}

}

![image](https://github.com/Preet-Sawant-9/recursion/assets/130697042/ae76f635-b932-43d2-8457-3a84122812f7)


Working of Recursion

Recursion performs a number of repetitive calls to the function from within the function. The recursive condition performs the repeating calls to the function until the base case is met.The base case is present inside the function, and once the condition of the base case is satisfied, it stops the execution.

Let’s understand it with a simple example.

![image](https://github.com/Preet-Sawant-9/recursion/assets/130697042/868d8633-0c60-4772-9528-d152f61587b7)


In the factorial function, we have to perform many repetitive calls to the function. In this example, the recursive condition would be n*factorial(n-1); factorial is the function's name, and the value of n is 5.

![image](https://github.com/Preet-Sawant-9/recursion/assets/130697042/ae594d43-b2f8-4dd0-a24e-67c07d0c898c)


First, in this function, 5 will be multiplied with factorial(5-1), then 4 is passed to the function. Similarly, in the next iteration, 4 is multiplied with factorial(4-1). This will continue till the value of n becomes 1.

THEORY
Algorithm: Factorial Calculation
Input: An integer 'n' for which you want to calculate the factorial. Output: The factorial of 'n'.

Start with a function named 'factorial' that takes an integer 'n' as its argument.
Inside the 'factorial' function: a. Check the base case: If 'n' is 0 or 1, return 1 because the factorial of 0 and 1 is 1. b. If 'n' is greater than 1, calculate the factorial recursively as follows:
Multiply 'n' by the result of the 'factorial' function with argument 'n - 1'.
Return this result.
In the 'main' function: a. Declare an integer 'num' to store the input number for which you want to calculate the factorial. b. Ask the user to input the value of 'num'. c. Call the 'factorial' function with 'num' as the argument to compute the factorial. d. Display the result as the factorial of 'num'.
Algorithm: Sum of Integers from 1 to n
Algorithm: Sum of Integers from 1 to n Using Recursive Function

Input: A positive integer 'n'. Output: The sum of all integers from 1 to 'n'.

Initialize a recursive function 'sumOfIntegers' that takes an integer 'n' as its argument.
In the 'sumOfIntegers' function: a. Check the base case: If 'n' is 1, return 1 because the sum of integers from 1 to 1 is 1. b. If 'n' is greater than 1, calculate the sum recursively as follows:
Return 'n' plus the result of the 'sumOfIntegers' function with argument 'n - 1'.
In the 'main' function: a. Declare an integer variable 'n' to store the input value for which you want to calculate the sum. b. Ask the user to input the value of 'n'. c. Call the 'sumOfIntegers' function with 'n' as the argument to compute the sum. d. Display the result as the sum of integers from 1 to 'n'.
Algorithm: Print String in Reverse Using Recursive Function
Input: A string 'str' and the length of the string 'n'. Output: Print the characters of 'str' in reverse order.

Initialize a recursive function 'printReverseString' that takes two arguments: 'str' and 'n'.
In the 'printReverseString' function: a. Check the base case: If 'n' is 0 (the string is empty), return. b. Print the last character of 'str' (str[n-1]). c. Call the 'printReverseString' function recursively with 'str' excluding the last character (str[0 to n-2]) and 'n-1' as arguments.
In the 'main' function: a. Declare a character array 'str' to store the input string. b. Read the input string into 'str'. c. Calculate the length of the input string and store it in 'n'. d. Call the 'printReverseString' function with 'str' and 'n' as arguments to print the string in reverse order
OUTPUT

Algorithm: Factorial Calculation
![image](https://github.com/Preet-Sawant-9/recursion/assets/130697042/7e039409-d3cf-42c0-8f99-eb407c23559a)


Algorithm: Sum of Integers from 1 to n
![image](https://github.com/Preet-Sawant-9/recursion/assets/130697042/2803a5e5-1055-4782-887f-324fb13f75cd)


Algorithm: Print String in Reverse Using Recursive Function
![image](https://github.com/Preet-Sawant-9/recursion/assets/130697042/449a8671-a833-4f65-914f-78b815fde6a0)
