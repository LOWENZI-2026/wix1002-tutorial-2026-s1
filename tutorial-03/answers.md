
# Tutorial 03 — Answers

## Question 1
a. 
```java
public class TUTORIAL_3 {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        if(3*8==27){
            System.out.println(" 3 x 8 is equal to 27 ");
        }
        else{
            System.out.println(" 3 x 8 is not equal to 27. ");
        }
    }
}
```
b.
```java
import java.util.Scanner;    
    public class TUTORIAL_3 {
    public static void main(String[] args) { 
    Scanner input = new Scanner(System.in);
        System.out.println(" Enter an integer ");
        int integer = input.nextInt();
        if (integer % 2 ==0 ){
            System.out.println(" The number is even number");
        }
        else{
            System.out.println(" The number is odd number");
        }
    }
}
```

c.
```java
import java.util.Scanner;    
    public class TUTORIAL_3 {
    public static void main(String[] args) { 
    Scanner input = new Scanner(System.in);
        System.out.println(" Enter a letter ");
        char letter = input.next().charAt(0);
        if (Character.isUpperCase(letter)){
            System.out.println(" The character is capital letter.");
        }
        else{
            System.out.println(" The character is not capital letter.");
        }
    }
}
```

d.
```java
import java.util.Scanner;    
    public class TUTORIAL_3 {
    public static void main(String[] args) { 
    Scanner input = new Scanner(System.in);
            System.out.println(" Enter sentence 1");
              String sen1 = input.nextLine();
            System.out.println(" Enter sentence 2");
              String sen2 = input.nextLine();  
         if (sen1.compareToIgnoreCase(sen2) < 0) {
             System.out.println(sen1 + "\n" + sen2);
          } 
         else {
               System.out.println(sen2 + "\n" + sen1);
         }
     }
}
```

e.
```java
import java.util.Scanner;    
    public class TUTORIAL_3 {
    public static void main(String[] args) { 
    Scanner input = new Scanner(System.in);  
        System.out.println(" Enter number (0-6): ");
        int num = input.nextInt();
        switch (num){
            case 0 : System.out.println(" Sunday ");
            break;
            case 1 : System.out.println(" Monday ");
            break;
            case 2 : System.out.println(" Tuesday ");
            break;
            case 3 : System.out.println(" Wednesday ");
            break;
            case 4 : System.out.println(" Thursday ");
            break;
            case 5 : System.out.println(" Friday ");
            break;
            case 6 : System.out.println(" Saturday ");
            break;
            default : System.out.println(" Invalid day ");
        }
    }
}
```

## QUESTION 2
a.
```java
if (num1 == num2){
         System.out.println("Number 1 is equal to number 2.");
    }    
      else{
          System.out.println("Number 1 is not equal to number 2.");
      }
```

b.
```java
if (x > y && x > z) {
        System.out.println("x is the largest number");
    }
else {
        System.out.println("x is not the largest number");
      }
```

c.
```java
String s1, s2;
if (s1.equals(s2)){
         System.out.println("They are equal strings.");
     }
else{
        System.out.println("They are not equal strings.");
     } 
```

d.
```java
if ( x >0 || y > 0){
        System.out.println("Either x or y is positive");
    }
else{
        System.out.println(" Neither x nor y is positive");
    }
```

## QUESTION 3
a.
```java
#####
$$$$$
```

b.
```java
#####
$$$$$
```

c.
```java
#####
```

d.
```java
no output
```

## QUESTION 4
``` java
import java.util.Scanner;    
    public class TUTORIAL_3 {
    public static void main(String[] args) { 
    Scanner input = new Scanner(System.in);
      
        System.out.println(" Enter number 1");
        int num1 = input.nextInt();
        System.out.println(" Enter number 2");
        int num2 = input.nextInt();
        System.out.println(" Enter number 3");
        int num3 = input.nextInt();
        
        int max = num1;

          if (num2 > max) {
             max = num2;
              }

          if (num3 > max) {
              max = num3;
            }

          System.out.println("The biggest number is " + max);
    }
}
```

## QUESTION 5
```java 
import java.util.Scanner;    
    public class TUTORIAL_3 {
    public static void main(String[] args) { 
    Scanner input = new Scanner(System.in);
        System.out.println(" Enter year ");
        int year = input.nextInt();
        if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {
          System.out.println(year + " is a leap year.");
        } 
        else {
          System.out.println(year + " is not a leap year.");
        }
    }      
}
```