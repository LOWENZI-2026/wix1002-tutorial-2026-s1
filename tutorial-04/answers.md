
# Tutorial 03 — Answers

## Question 1
a. 
```java 
public class TUTORIAL_4 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        for (int n = 0; Math.pow (n,3)< 2000;n++){
            System.out.println(n);
        }
    }
}
```

b.
```java 
public class TUTORIAL_4 {
    public static void main(String[] args) {
        for ( int i = 1 ; i<= 12 ; i++){
            int num = (int) Math.pow(i, 2);
            System.out.println(num);
        }
    }
}
```
c.
```java
import java.util.Random;
  public class TUTORIAL_4 {
    public static void main(String[] args) {
        Random ran = new Random();
          int num = ran.nextInt(101);
          for (int i =0 ; i < 4; i++){
              for ( int y = 0 ; y < 5 ; y++){
                  System.out.print(num);
              }
              System.out.println();
          }
    }
}
```

d.
```java 
import java.util.Scanner;

public class TUTORIAL_4 {
    public static void main(String[] args) {

        Scanner input = new Scanner(System.in);
        System.out.println(" Enter a number ");
        int num = input.nextInt();
        int sum = 0;
        for ( int i = 1 ; i <= num ; i++){
            sum = sum + (i + num);           
        }
        System.out.println("The sum of numbers is " + sum);
    }
}
```

e.
```java
public class TUTORIAL_4 {
    public static void main(String[] args) {
        
        double sum = 0 ;
        for (double i = 1 ; i <= 25 ; i++){
            double num = i / (26-1);
            sum = sum + num ;
            System.out.printf( "The sum is % .2f\n", sum);
        }  
        System.out.printf( "The total sum is % .2f\n", sum);
    }
}
```

## Question 2
a.
```java

       for (int x = 10; x > 0; x--)
       sum += x; 
```
b.
```java
        int x =0 ;
         int y =0 ;
         do{
          x += 2 ; 
          y += x ;
              
            System.out.println(x + " and " + y);

         }while(x < 100);
```
c. 
```java
        for ( int x=1,y =20; x < y ; x++, y-=2)
            System.out.println(x + " " + y);
```

d. 
```java
        int i = 1;
           while(i<10) {
              i++;
              if (i==10)
               System.out.println("Program End");
           }
```
## QUESTION 3 
```java
public class TUTORIAL_4 {
    public static void main(String[] args) {
        int f1 = 1;
           int f2 = 1;
           System.out.println(" The value of F1 is " + f1);
           System.out.println(" The value of F2 is " + f2);
           for (int i = 3; i <= 10 ; i++){
               int fn = f1 + f2; 
               System.out.println(" The value of F" + i + " is " + fn);
               f1 = f2;
               f2 = fn ;
           }
    }
}
```

## QUESTION 4
```java 
import java.util.Scanner;
public class TUTORIAL_4 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        System.out.println(" Enter a sentence ");
           String sent = input.nextLine(); 
             for (int i = sent.length() - 1; i >= 0; i--) {
                System.out.print(sent.charAt(i));
                } 
             System.out.println();
    }
}
```