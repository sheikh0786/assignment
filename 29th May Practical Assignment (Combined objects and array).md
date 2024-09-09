# Practical Assignment in Array in Java (PW)
###  Write a program to demonstrate method overloading with 3 different parameters.
```java
import java.util.*;
class Sum
{
   public int add(int a , int b)
    {
      return a+b;
    }

    public int add(int a , int b , int c)
    {
        return a+b+c;
    }
}

class methodOverloading
{
    public static void main(String args[])
    {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter two numbers:");
        int a = sc.nextInt();
        int b = sc.nextInt();
        Sum sum = new Sum();
        int c = sum.add(a,b);
        int d = sum.add(a,b,c);
        System.out.println( "a+b= c:" +c);
        System.out.println("a + b + c = d:" +d);
        System.out.println("Metod Overloading");
        sc.close();
    }
}
```

### Write a program to create an object of an class which contain a method and call that class method in main method.

```java
public class objectCall 
{
    public void message()
    {
        System.out.println("This message is from message method");
    }
    public static void main(String[] args) 
    {
        objectCall obj = new objectCall();
        obj.message();
       
    }    
}

```

### Write a Java program to calculate the sum of all elements in an integer array?
```java
public class sumArray 
{
    public static void main(String[] args) 
    {
        int arr[] = {2,4,1,5,7};
        int sum=0;

        for(int i =0; i < arr.length; i++)
        {
            sum = sum + arr[i];
        }

        System.out.println(sum);
    }    
}
```


### Write a Java program to find the index of a specific element in an integer array.?
// This program i solved by little complex method for better understanding i used user input and i print every output in this code 

```java
import java.util.*;

public class arrayIndex {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("======================================================");
        System.out.println("Enter the number of element you want to Enter in array");

        int len = sc.nextInt();

        int arr[] = new int[len]; // entering size of array by user

        System.out.println("======================================================");
        System.out.println("Enter " + len + " number for an array:");
        System.out.println("======================================================");
        for (int i = 0; i < len; i++) { // entering number one by one in array
            System.out.println("Enter " + i + " index number for an array:");
            arr[i] = sc.nextInt();
        }
        System.out.println("======================================================");
        System.out.println("The number for an array you  entered are:");

        for (int i = 0; i < arr.length; i++) {
            System.out.println(+arr[i]); // displaying numbers user entered in array
        }
        System.out.println("======================================================");
        System.out.println("Enter the number you want to search index");
        int target = sc.nextInt();
        System.out.println("======================================================");
        int index = -1;
        for (int i = 0; i < arr.length; i++) {
            if (arr[i] == target) { // searching the number is in array or not
                index = i;
                break;
            }
        }
        if (index != -1) {
            System.out.println("The number you enter is in array of index:" + index);
        } else {
            System.out.println("The number you entered in not in araay");
        }

        System.out.println("======================================================");

        sc.close();
    }

}
```

### Write a Java program to print an entire array?
```java
public class printArray 
{
    public static void main(String[] args) 
    {
        int arr[] = {2,3,4,6,8};
        for(int i=0; i<arr.length; i++)
        {
            System.out.println(arr[i]);
        }
    }    
}
```
