
# Tutorial 01 — Answers

## Part I

### Question 1

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
| Two numbers (num1, num2) | Multiply num1 and num2 | The multiplication result |

2. Pseudocode:

```text
Start
    Read num1, num2
    result ← num1 * num2
    Print result
End
```

3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[/"Read num1, num2"/]
    B --> C["result = num1 * num2"]
    C --> D[/"Print result"/]
    D --> E([End])
```
### QUESTION 2

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|A random number| Compare n > 50 | comparison result (greater or not greater) |

2. Pseudocode:

```text
Start
Generate a random number, n
    If n > 50 then
        Print "The number is greater than 50"
    Else
        Print "The number is not greater than 50"
    End If
End
```
3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B["Generate random number, n"]
    B --> C{n > 50?}
    C -->|Yes| D[/Print "The number is greater than 50"/]
    C -->|No| E[/Print "The number is not greater than 50"/]
    D --> F([End])
    E --> F
```
### QUESTION 3 

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|User's mark| compare mark >= 40 , mark is 0-100 | pass, fail, invalid mark |

2. Pseudocode:

```text
Start
Read mark
    If mark <0 or > 100 then
        Print "Invalid mark"
    Else if mark >= 40
        Print "Pass"
    Else
        Print "Fail"
    End If
End
```
3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[/Read mark/]
    B --> C{mark <0 or mark > 100?}
    C -->|Yes| D[/Print "Invalid mark"/]
    C -->|No| E{mark >= 40?}  
    E -->|Yes| F[/Print "Pass"/]
    E -->|No| G[/Print " Fail"/]
    D --> H([End]) 
    F --> H
    G --> H
```

### QUESTION 4

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|Random number of dice values in 0-6 of player 1 and player 2| compare dice value of player 1 and player 2| win, draw |

2. Pseudocode:

```text
Start
 Generate dice value for player 1 (p1)
 Generate dice value for player 2 (p2)
    If p1 > p2 then
        Print "Player 1 wins"
    Else If p2 > p1 then
        Print "Player 2 wins"
    Else
        Print "It is a draw"
    End If
End
```
3. Flow chart :
   
```mermaid 
graph TD
    A([Start]) --> B[Generate dice values for p1 and p2]
    B --> C{p1 > p2?}
    C -->|Yes| D[/Print "Player 1 wins"/]
    C -->|No| E{p2 > p1?}
    E -->|Yes| F[/Print "Player 2 wins"/]
    E -->|No| G[/Print "It is a draw"/]
    D --> H([End])
    F --> H
    G --> H
```

### QUESTION 5

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|Length and width| Perimeter = 2 × (length + width)| perimeter of rectangle |

2. Pseudocode:

```text
Start
    Read length, width
    Calculate perimeter ← 2 * (length + width)
    Print perimeter
End
```

3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[/Read length, width/]
    B --> C["perimeter = 2 * (length + width)"]
    C --> D[/Print perimeter/]
    D --> E([End])
```

### QUESTION 6

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|10 random numbers| Loop 10 times to generate numbers and compare each with the current minimum to find the smallest| Minimum number |

2. Pseudocode:

```text
Start
Set counter ← 1
    Generate first random number, min_num
    While counter < 10
        Generate new random number, num
        If num < min_num then
            min_num ← num
        End If
        counter ← counter + 1
    End While
    Print min_num
End
```
3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[counter = 1]
    B --> C[Generate min_num]
    C --> D{counter < 10?}
    D -->|Yes| E[Generate num]
    E --> F{num < min_num?}
    F -->|Yes| G[min_num = num]
    F -->|No| H[counter = counter + 1]
    G --> H
    H --> D
    D -->|No| I[/Print min_num/]
    I --> J([End])
```
### QUESTION 7

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|10 random numbers in 10–100| Loop 10 times to generate numbers (10-100),test n % 2 == 0 to identify even or odd| Total count of even number and odd number|

2. Pseudocode:

```text
Start
Set even_count ← 0, odd_count ← 0, counter ← 0
    While counter < 10
        Generate random number (num) between 10 and 100
        If num % 2 == 0 then
            even_count ← even_count + 1
        Else
            odd_count ← odd_count + 1
        End If
        counter ← counter + 1
    End While
    Print even_count, odd_count
End
```

3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[even_count = 0, odd_count = 0, counter = 0]
    B --> C{counter < 10?}
    C -->|Yes| D[Generate num between 10-100]
    D --> E{num % 2 == 0?}
    E -->|Yes| F[even_count = even_count + 1]
    E -->|No| G[odd_count = odd_count + 1]
    F --> H[counter = counter + 1]
    G --> H
    H --> C
    C -->|No| I[/Print even_count, odd_count/]
    I --> J([End])
```

## Part II

### Question 8

 1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|A sentence|Count 'U' and 'M'|Number of  'U' and 'M'|

2. Pseudocode:

```text
Start
Set countU ← 0, countM ← 0,index ← 0
    Read sentence
    WHILE index < LENGTH(sentence) DO
    ch ← CHARACTER_AT(sentence, index)
        If character == 'U' then
            countU ← countU + 1
        Else if character == 'M' then
            countM ← countM + 1
        End If
        index ← index + 1
    END WHILE
    Print countU, countM
End
```
3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[countU = 0, countM = 0,index =0]
    B --> C[/Read sentence/]
    C --> D{"index < LENGTH(sentence)?"}
    D -->|Yes| E[/Get next character/]
    E --> F{character == 'U'?}
    F -->|Yes| G[countU = countU + 1]
    F -->|No| H{character == 'M'?}
    H -->|Yes| I[countM = countM + 1]
    H -->|No| J[Continue]
    G --> K[index = index + 1]
    I --> K
    J --> K
    G --> D
    I --> D
    J --> D
    D -->|No| L[/Print countU, countM/]
    L --> M([End])
```

### QUESTION 9

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|Webpage content,keyword|Search the web page content for the keyword and count how many times it appears|Frequency of a keyword|

2. Pseudocode:

```text
Start
Set frequency = 0
    Read web_page_content, keyword
    While keyword is found in web_page_content
        frequency = frequency + 1
        Move to the next search position
    End While
    Print frequency
End
```

3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[frequency = 0]
    B --> C[/Read web_page_content, keyword/]
    C --> D{Keyword found?}
    D -->|Yes| E[frequency = frequency + 1]
    E --> F[Move to next position]
    F --> D
    D -->|No| G[/Print frequency/]
    G --> H([End])
```

### QUESTION 10

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|List of 100 students| Loop 100 times, check if the student's gender is female  and increment the counter|Number of female students |

2. Pseudocode:

```text
Start
Set female_count = 0, counter = 0
    While counter < 100
        Read student_gender
        If student_gender == "female" then
            female_count = female_count + 1
        End If
        counter = counter + 1
    End While
    Print female_count
End
```

3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[female_count = 0, counter = 0]
    B --> C{counter < 100?}
    C -->|Yes| D[/Read student_gender/]
    D --> E{student_gender == female?}
    E -->|Yes| F[female_count = female_count + 1]
    E -->|No| G[counter = counter + 1]
    F --> G
    G --> C
    C -->|No| H[/Print female_count/]
    H --> I([End])
```

### QUESTION 11

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|5 random numbers | Store the numbers in a list and sort the list in descending order|Descending list |

2. Pseudocode:

```text
Start
 // Phase 1: Generate and store 5 numbers
    Initialise a counter as 1
    While the counter is less than or equal to 5
        Randomly generate a number
        Store the number in a list
        Increase the counter by 1
    End While

// Phase 2: Bubble sort in descending order
    Initialise an iteration as 1
    While the iteration is less than the total number in the list
        For each number in the list
            If the current number is less than the next number then
                Assign the current number to the temporary number
                Assign the next number to the current number
                Assign the temporary number to the next number
            End If
        End For
        Increase iteration by 1
    End While

// Phase 3: Print the sorted list
    For each number in the sorted list
        Print the number
    End For
End
```

3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[counter = 1]

    %% Phase 1: Generate 5 numbers
    B --> C{counter <= 5?}
    C -->|Yes| D[/Randomly generate a number/]
    D --> E[Store the number in a list]
    E --> F[counter = counter + 1]
    F --> C

    %% Phase 2: Bubble Sort
    C -->|No| G[iteration = 1]
    G --> H{iteration < total number in list?}
    H -->|Yes| I[Get first pair in list]
    I --> J{current number < next number?}
    J -->|Yes| K[temp = current<br>current = next<br>next = temp]
    J -->|No| L[Move to next pair]
    K --> L
    L --> M{Checked all pairs?}
    M -->|No| J
    M -->|Yes| N[iteration = iteration + 1]
    N --> H

    %% Phase 3: Print sorted list
    H -->|No| O[Get first number in sorted list]
    O --> P{More numbers in list?}
    P -->|Yes| Q[/Print the number/]
    Q --> R[Move to next number]
    R --> P
    P -->|No| S([End])
```

### QUESTION 12

1. IPO Model:

| Input | Process | Output |
| :--- | :--- | :--- |
|User's guess| Compare user's guess with target|Higher, Lower or Correct |

2. Pseudocode:

```text
Start
Generate a random number
    Read user_guess
        If user_guess < random_number then
            Print "lower"
        Else if user_guess > random_number
            Print "higher"
        Else
            Print "correct"
    End if
End
```

3. Flow chart :
   
```mermaid
graph TD
    A([Start]) --> B[Generate a random number]
    B --> C[/Read user_guess/]
    C --> D{user_guess == random_number?}
    D -->|No| E{user_guess < random_number?}
    E -->|Yes| F[/Print "lower"/]
    E -->|No| G[/Print "higher"/]
    F --> C
    G --> C
    D -->|Yes| H[/Print "correct"/]
    H --> I([End])
```