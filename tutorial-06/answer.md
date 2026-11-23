# Tutorial 6 — Answers

## Question 1
a.
```java 

 public static int getMax(int a, int b, int c) {
    int max = a;
    if (b > max) {
        max = b;
    }
    if (c > max) {
        max = c;
    }
    return max;
}
```
b.
```java    
    public static boolean isSquare(int num) {
    if (num < 0) {
        return false;
    }
    int root = (int) Math.sqrt(num);
    return root * root == num;
}
```
c.
```java
    public static long factorial(int num) {
    long fact = 1;
    for (int i = 2; i <= num; i++) {
        fact *= i;
    }
    return fact;
}

public static long combination(int n, int k) {
    if (k < 0 || k > n) {
        return 0;
    }
    return factorial(n) / (factorial(k) * factorial(n - k));
}
```

d
```java
    public static boolean isPentagonal(int num) {
    if (num <= 0) {
        return false;
    }
    int n = 1;
    int pentagonal = 0;
    while (pentagonal < num) {
        pentagonal = n * (3 * n - 1) / 2;
        if (pentagonal == num) {
            return true;
        }
        n++;
    }
    return false;
}
```
e.
```java
    public static void displayLettersAndDigits(String str) {
    int letters = 0;
    int digits = 0;

    for (int i = 0; i < str.length(); i++) {
        char ch = str.charAt(i);
        if (Character.isLetter(ch)) {
            letters++;
        } else if (Character.isDigit(ch)) {
            digits++;
        }
    }

    System.out.println("Number of letters: " + letters);
    System.out.println("Number of digits: " + digits);
}
```
f.
```java
    import java.util.Random;

public static void generateRandomNumbers(int[] numbers) {
    Random rand = new Random();
    for (int i = 0; i < 10 && i < numbers.length; i++) {
        numbers[i] = rand.nextInt(101); // 0 to 100 inclusive
    }
}
```
g.
```java
    public static void calculateCircle(double radius, double[] results) {
    results[0] = Math.PI * radius * radius; 
    results[1] = 2 * Math.PI * radius;      
}
```
h.
```java
    import java.util.Random;

public static int firstDuplicateRandom() {
    Random rand = new Random();
    boolean[] seen = new boolean[11]; 

    while (true) {
        int num = rand.nextInt(11); 
        if (seen[num]) {
            return num;
        }
        seen[num] = true;
    }
}
```
## Question 2 
```java
    import java.util.Scanner;

public class DecreasingOrder {

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter three numbers: ");
        double num1 = scanner.nextDouble();
        double num2 = scanner.nextDouble();
        double num3 = scanner.nextDouble();

        displayDecreasing(num1, num2, num3);

        scanner.close();
    }

    public static void displayDecreasing(double a, double b, double c) {
        double temp;

        if (a < b) {
            temp = a;
            a = b;
            b = temp;
        }
        if (a < c) {
            temp = a;
            a = c;
            c = temp;
        }
        if (b < c) {
            temp = b;
            b = c;
            c = temp;
        }

        System.out.println("Numbers in decreasing order: " + a + ", " + b + ", " + c);
    }
}
```