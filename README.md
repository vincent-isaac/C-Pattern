# Pattern

## Aim: To write a C# program for a pascal's triangle.

## Algorithm:

###Step 1: 
Start.

###step 2:
Get the user input for the triangle size.

###step 3:
Create a nested 'for loop', Outer loop for rows and inner for loop for printing values.

###Step 4:


## Program:
```c#
namespace program4;
    public class Class1
    {
        static void Main(string[] args)
        {
            int num,value=1;
            Console.WriteLine("Enter the size of the pascal's triangle :");
            num=Convert.ToInt32(Console.ReadLine());
            for(int i =0;i<num;i++)
            {
                for(int space=0;space<num-i;space++)
                    Console.Write(" ");
                for(int j=0;j<=i;j++)
                {
                    if(i==0 || j==0)
                        value=1;
                    else
                        value=value*(i-j+1)/j;
                    Console.Write(value+" ");
                }
            Console.WriteLine();
                
            }        
        }
    }
```
## Output:

![c# ex3](https://user-images.githubusercontent.com/75234588/189466049-6aa61089-3c5d-4ca9-8531-a04a05b1a790.PNG)

## Result: 
Thus the C# program to display for a pascal's triangle is executed successfully.
