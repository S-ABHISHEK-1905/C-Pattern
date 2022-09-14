# Pattern

## Aim:
To write a C# program to print the pascal triangle

## Algorithm:
### Step-1: 
Start
### Step-2: 
Declare variables rows,val,i,j,blank
### Step-3: 
Initialize the value of variables, i=0,j=0,val=1
### Step-4: 
Enter the limit
### Step-5: 
using for loop printing " " when i&j==0 and using for loop applying the concept of pascal triangle

##Program:
~~~
using System;
namespace PascalTriangleDemo
{
    class Example
    {
        public static void Main()
        {
            int rows = 5, val = 1, blank, i, j;
            for (i = 0; i < rows; i++)
            {
                for (blank = 1; blank <= rows - i; blank++)
                    Console.Write(" ");
                for (j = 0; j <= i; j++)
                {
                    if (j == 0 || i == 0)
                        val = 1;
                    else
                        val = val * (i - j + 1) / j;
                    Console.Write(val + " ");
                }
                Console.WriteLine();
            }
        }
    }
}
~~~

## Output:
![image](https://user-images.githubusercontent.com/66360846/190067423-529e79e6-18c3-4b26-8b66-de12ade19d3c.png)


## Result:
Thus the C# program to display pascal triangle is exucuted sucessfully.
