
# Tutorial 5 — Answers

## Question 1
a. 
```java 
 float[] floatArray = new float[12];
 ```
b.
```java 
char[] letter = {'A','B','C','D','E'};
```

c.
```java
String[] studentName = new String[100];
```

d.
```java 
int [][] table = new int[6][2];
```

e.
```java
int [][] matrixArray = {{6,9},{2,5},{4,6}};
```

f.
```java 
 matrixArray[1][1] = 4;
 matrixArray[2][0] = 3;
 matrixArray[2][1] = 7;
```

g.
```java 
 for (int i = 0; i < nameContact.length; i++) {
          System.out.println(nameContact[i]);
 }
```
## Question 2
a.
```java
String[] code = {"AAA", "AAB", "AAC", "AAD"};
```

b.
```java   
   int[] num = new int[10];
    for(int k=0; k<num.length; k++)
    sum+=num[k];
```

c.
```java 
     int [][] t = new int[3][3];
     t[1][2] = 5;
```

d.
```java      
     int i=4;
     int []score = new int[5];
     score [1] = 78;
     score[i] = 100;
```

## Question 3
```java
     {0, 0, 0, 0, 0}
     {12, 0, 0, 0, 0}
     {12, 31, 0, 0, 0}
     {961, 31, 0, 0, 0}
     {961, 31, 0, 31, 0}
     {961, 31, 1, 31, 0}
     {961, 31, 1, 31, 31}
        FINAL
         marks[0] = 961
         ​marks[1] = 31
         ​marks[2] = 1
         ​marks[3] = 31
​         marks[4] = 31
```

## Question 4
```java 
 int count = 0;
     for (int i = 0; i < sentence.length; i++) {
     if (sentence[i].equals("the")) { 
        count++;
     }
    }
        System.out.println("Occurrences of \"the\" : " );
```

## Question 5
```java 
     for (int m = sentence.length  - 1; m >= 0; m--) {
        String currentWord = sentence[m];
        String reversedWord = " ";
  
        for (int n = currentWord.length() - 1; n >= 0; n--) {
        reversedWord += currentWord.charAt(n);
        }
           System.out.println(reversedWord);
}
```

## Question 6
```java 
int number = r.nextInt(256); 
       System.out.println("Random Number: " + number);
       
       int[] binary = new int[8];
       int temp = number;
       
       for (int i = 7; i >= 0; i--) {
       binary[i] = temp % 2;
       temp = temp / 2;
       }
       
       System.out.print("Binary: ");
       for (int i = 0; i < binary.length; i++) {
       System.out.print(binary[i]);
       }
```