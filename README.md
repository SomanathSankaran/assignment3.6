# assignment3.6
QN 1 Can you overload a method with the same return type? Explain your answer with proper logic 1.YES we can overload a method with same return type by changing the number of parameters.Take the case if we want to find the performance of student in 2 main subjects and suppose we want to find the total of other subjects also. In this case we can use two sum methods with different parameters and find the students' performance 2.If we overlad with different return type it will be confusing for the compiler to call which method import java.util.Scanner;

public class acad {

public static void main(String[] args) {
    // TODO Auto-generated method stub
Scanner in=new Scanner(System.in);//scanner used for getting input from user through keybaord System.out.println("Enter name"); String name=in.next(); System.out.println("Enter marks"); int number1=in.nextInt();//getting input at runtime int number2=in.nextInt();//getting input at runtime int number3=in.nextInt();

acad a=new acad();//creating object a to call non staic method sum inside static method acad a1=new acad(); a.sum(number1,number2);//calling the static method sum which accepts 2 parameters(number1,number2) a1.sum(number1,number2,number3);//calling the method which accepts 3 parameters

}

// Overloading – Different Number of parameters

public void sum(int a,int b)
{
    int sum=a+b;

    System.out.println("Sum of 2 main subject:"+sum);
}
public void sum(int a,int b,int c)
{
    int sum=a+b+c;
    System.out.println("Sum of 3 subjects(including optional subject):"+sum);

}
} QN 2. Write a program in Java using Arrays, that sorts the element in a descending order.

import java.util.Arrays; import java.util.Scanner;

public class acad {

public static void main(String[] args) {
Scanner in=new Scanner(System.in);
System.out.println("Enter the no of elements in the array "); 
int n=in.nextInt(); 
int[] a=new int[n];
System.out.println("Enter the numbers");
for(int m=0;m<n;m++)
{
    a[m]=in.nextInt();
}
//sort the array in ascending order using sort
Arrays.sort(a);
//print  the elements in descending order
System.out.println("Array sorted in descending order");
for(int m=(a.length-1);m>=0;m--)

{ System.out.println(a[m]);

} } }
