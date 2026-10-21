
# Tutorial 02 — Answers

## Question 1
a. 
```java
public class TUTORIAL_2 {
    public static void main(String[] args) {
        System.out.print(" Faculty of ");
        System.out.print(" Computer Science and Information Technology ");
    }
}
```

b.
```java
public class TUTORIAL_2 {
    public static void main(String[] args) {        
        System.out.print(" Faculty of \n Computer Science \n and \n Information Technology\n");
    }
}
```
## Question 2
```java
public class TUTORIAL_2 {
    public static void main(String[] args) {
        System.out.println(" \"SDN \"- Software-defined networking");
    }
}
```
## Question 3
a.
```java
public class TUTORIAL_2 {
   public static void main(String[] args) {   
         System.out.println("Java Programming");
   }
}
```

b.
```java
public class TUTORIAL_2 {
    public static void main(String[] args) { 
         System.out.println("Introduction to Java!");
    }
}
```

c.
```java
public class TUTORIAL_2 {
    public static void main(String[] args) { 
         System.out.println("\\t is the horizontal tab character");
    }
}
```

d.
```java
public class TUTORIAL_2 {
    public static void main(String[] args) { 
         System.out.println("Java is case sensitive!" );
    }
}
```

## Question 4
a.
```java
        String matricNumber; 
```

b.
```java
        double pi;
```

c,
```java
        boolean M = false;
```

d.
```java
        long P = 8800000000L;
```

e,
```java
       char letter ='U';
```

f.
```java
       final String PRO = "Java";
```
## Question 5
a.
```java
       double AMOUNT = 32.5;
       AMOUNT += 10;
       System.out.println(" The amount is " + AMOUNT);
```
b.
```java
       String chapter = "Summary";
       System.out.println(chapter);
```

c.
```java
       int num = 0;
       ++num;
       num++;
       int num1 = num;
```
d. 
```java
      double num = 3000;
       System.out.printf("%4.2f\n", num);
```

e.
```java
       String contact;
       Scanner keyboard = new Scanner(System.in);
       contact = keyboard.nextLine();
```

## Question 6
```java
import java.util.Scanner;
public class TUTORIAL_2 {
    public static void main(String[] args) {  
    Scanner sc = new Scanner(System.in);
        System.out.println(" Enter diameter ");
        double diameter = sc.nextDouble();
        double circumferenceCircle = 2 * Math.PI * (diameter/2.0);
        System.out.printf("The circumference of a circle is : %.3f \n " , circumferenceCircle );
    }
}
```
## Question 7
```java
import java.util.Scanner;
public class TUTORIAL_2 {
    public static void main(String[] args) {
    Scanner sc = new Scanner(System.in);
         System.out.println(" Enter inches ");
         double inches =  sc.nextDouble();
         double meter = inches * (2.54/100.0);
         System.out.printf("20.17 inches = %.2f meters \n", meter);
         
    }
}
```