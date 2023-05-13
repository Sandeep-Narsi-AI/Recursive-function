# Recursive-function

## Aim: 
To write a C# program to reverse a number using recursive function.

## Algorithm:
### Step1:
Create a function for reversing.

### Step2:
Get the number from the user.

### Step3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

### Step4:
Recusively call this function to get the reversed number.

### Step5:
print the reversed number.

## Program:
```
Name   : P.SANDEEP
REG.NO : 212221230074
```
~~~
using System;

namespace Recursive_Function
{
    class Program
    {
        public static int m, reverse = 0;
        public static int Recur(int number)
        {

            if (number > 0)
            {
                Program.m = number % 10;
                Program.reverse = Program.reverse * 10 + m;
                number = number / 10;
                return Recur(number);
            }
            return Program.reverse;

        }
        static void Main(string[] args)
        {
            int num;
            Console.Write("Enter the Number       : ");
            num = Convert.ToInt32(Console.ReadLine());
            Console.Write("The Reversed Number is : ");
            Console.WriteLine(Recur(num));
        }
    }
}
~~~

## Output:
![output](output.png)


## Result:
C# program to reverse a number using recursive function is executed successfully.
