#### Constructors
```
In Java, a constructor is a block of codes similar to the method. It is called when an instance of the class is created. 
The constructor name must match the class name, and it cannot have a return type.
```

##### Take three constructors where the first constructor will calculate the area of a triangle, the second constructor will calculate the area of a rectangle, and the third constructor will calculate the area of a rhombus using an overloading constructor. However, Input must be taken from users.

```java
package com.mycompany.mavenproject1;

import java.util.Scanner;

/**
 *
 * @author sa1tama0
 */
public class Mavenproject1 {
    double result;
    Mavenproject1(int c,double a,double b)
    {
        if (c == 1 || c == 3)
        {
            result = (a * b)/2;
        } 
        else if (c == 2)
        {
            result = a * b;
        }
        else 
        {
            System.out.println("ERROR");
        }
        System.out.println("The result is : "+ result);
    }
    public static void main(String[] args) {
        Scanner scan = new Scanner(System.in);
        System.out.println("1. Triangle ");
        System.out.println("2. Rectrangle ");
        System.out.println("3. Rhombus ");
        int tr = scan.nextInt();
        System.out.println("Base/Length/Diagonal : ");
        double base= scan.nextDouble();
        System.out.println("Height/Width/Diagonal : ");
        double height= scan.nextDouble();
        Mavenproject1 obj = new Mavenproject1(tr,base,height);
    }
}
```
