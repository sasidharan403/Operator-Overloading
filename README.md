# Operator-Overloading

## Aim:
 To write a C# program to pass values through constructors(default and parameterized) and also overload equal operators by checking whether objects are equal using operator overloading. 
 
 ## Algorithm:
 ## Step1:
Create a class for operator overloading.

## Step2:
Get inputs for length,breadthandheight of the box fromthe user and then calculate the volume in overloading function.

## Step3:
After that return a new object for the calculated volume.

## Step4:
Then create a new object to store the return object.

## Step5:
After that print the calculated volume.
 
 
 ## Program:
 ~~~
 using System;
class example
{
   public int length, breadth, height, volume;
   public static example operator +(example e1, example e2)
   {
       
       example e3 = new example();
       e1.volume = e1.length * e1.breadth * e1.height;
       e2.volume = e2.length * e2.breadth * e2.height;
       e3.length = e1.length + e2.length;
       e3.breadth = e1.breadth + e2.breadth;
       e3.height = e1.height + e2.height;
       e3.volume = e3.length * e3.breadth * e3.height;
       return e3;
   }
   public static void Main()
   {
       example e1 = new example();
       Console.WriteLine("Enter the length of e1:");
       e1.length = Convert.ToInt32(Console.ReadLine());
       Console.WriteLine("Enter the breadth of e1:");
       e1.breadth = Convert.ToInt32(Console.ReadLine());
       Console.WriteLine("Enter the height of e1:");
       e1.height = Convert.ToInt32(Console.ReadLine());
       example e2 = new example();
       Console.WriteLine("Enter the length of e2:");
       e2.length = Convert.ToInt32(Console.ReadLine());
       Console.WriteLine("Enter the breadth of e2:");
       e2.breadth = Convert.ToInt32(Console.ReadLine());
       Console.WriteLine("Enter the height of e2:");
       e2.height = Convert.ToInt32(Console.ReadLine());
       example e4 = new example();
       e4 = e1 + e2;
       Console.WriteLine("Volume of e1:");
       Console.WriteLine(e1.volume);
       Console.WriteLine("Volume of e2:");
       Console.WriteLine(e2.volume);
       Console.WriteLine("Volume of e3:");
       Console.WriteLine(e4.volume);
   }
}
~~~
 
 ## Output:
 ![Screenshot (196)](https://github.com/sasidharan403/Operator-Overloading/assets/94154712/2027fcd3-583d-4ea8-83ae-234ac60388ce)

 
 ## Result:
 Thus, a C# program to find the volume of a box using operator overloading is executed sucessfully.
