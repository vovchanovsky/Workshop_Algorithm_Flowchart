# Workshop: Algorithm and Flowchart

For each question in this workshop, you must complete **two** things:

1.  **Write the pseudocode**
2.  **Draw the flowchart** using either
    - **Option 1:** Draw.io (recommended) → export image → upload to
      your repository → link it in this file
    - **Option 2 (optional):** Write a Mermaid flowchart directly in
      Markdown
    - **Option 3 (optional):** Any other valid method

👉 **IMPORTANT:** At the **bottom of each question**, add the
following sections:

### ✔ Pseudocode

### ✔ Flowchart

---

## 1. Check Even or Odd Number

Design an algorithm and flowchart that take a number as input and
determine whether it is even or odd.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number % 2 == 0 THEN
        PRINT Even
    ELSE
        PRINT Odd
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([Start]) --> I[/Get input N/]
    I --> B{N % 2 == 0 ?}
    B -->|Yes| C[/Print Even/]
    B -->|No| D[/Print Odd/]
    C --> E([End])
    D --> E([End])
```

---

## 2. Calculate Total and Average Marks

Write the algorithm and draw the flowchart for a program that inputs
marks for 3 subjects, calculates the total and average, and displays
both.

### ✔ Pseudocode

```text
START
    nunber_of_marks = 3
    count = 0, total = 0
    REPEAT number_of_marks TIMES
        count += 1
        PRINT "Enter mark #" count
        INPUT mark
        total += mark
    ENDREPEAT  
    average = total / number_of_marks
    PRINT "Total Marks: " total
    PRINT "Average Marks: " average
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[count = 0, total = 0,number_of_marks = 3]
    B --> C{count <  number_of_marks ?}
    C -->|Yes| D[count += 1]
    D --> E[/INPUT mark/]
    E --> F[total += mark]
    F --> C
    C -->|No| G[average = total / number_of_marks]
    G --> H[/PRINT total and average/]
    H --> I([END])
```

---

## 3. Display Multiplication Table

Create an algorithm and flowchart that input a number and display its
multiplication table from 1 to 10 using a loop.

### ✔ Pseudocode

```text
START
    INPUT number
    count = 1
    REPEAT 10 TIMES
        result = number * count 
        PRINT number "x" count "=" result
        count += 1
    ENDREPEAT
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT number/]
    B --> C[count = 1]
    C --> D{count <= 10 ?}
    D -->|Yes| E[result = number * count]
    E --> F[/PRINT number "x" count "=" result/]
    F --> G[count += 1]
    G --> D
    D -->|No| H([END])
```

---

## 4. Positive, Negative, or Zero Check

Write the algorithm and flowchart to input a number and display whether
it is positive, negative, or zero.

### ✔ Pseudocode

```text
START
    INPUT number
    IF number > 0 THEN
        PRINT "Positive"
    ELSE IF number == 0 THEN
        PRINT "Zero"
    ELSE
        PRINT "Negative"
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT number/]
    B --> C{number > 0 ?}
    C -->|Yes| D[/PRINT "Positive"/]
    C -->|No| E{number == 0 ?}
    E -->|Yes| F[/PRINT "Zero"/]
    E -->|No| G[/PRINT "Negative"/]
    D --> H([END])
    F --> H([END])
    G --> H([END])
```

---

## 5. Simple Interest Calculator

Create an algorithm and flowchart for a program that calculates simple
interest using the formula:

**SI = (P × R × T) / 100**

- **P = Principal** → original amount of money
- **R = Rate of Interest** → percentage per year
- **T = Time** → number of years

### ✔ Pseudocode

```text
START
    INPUT P, R, T
    SI = (P * R * T) / 100
    PRINT SI
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT P, R, T/]
    B --> C[SI = (P * R * T) / 100]
    C --> D[/PRINT SI/]
    D --> E([END])
```

---

## 6. Average Temperature Calculation

Write the algorithm and draw the flowchart for a program that takes the
temperature of 7 days, finds the average temperature, and displays it.

### ✔ Pseudocode

```text
START
    number_of_days = 7
    count = 0, total = 0
    REPEAT number_of_days TIMES
        count += 1
        PRINT "Enter temperature for day #" count
        INPUT temp
        total += temp
    ENDREPEAT  
    average = total / number_of_days
    PRINT "Average Temperature: " average
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[count = 0, total = 0,number_of_days = 7]
    B --> C{count <  number_of_days ?}
    C -->|Yes| D[count += 1]
    D --> E[/INPUT temp/]
    E --> F[total += temp]
    F --> C
    C -->|No| G[average = total / number_of_days]
    G --> H[/PRINT average/]
    H --> I([END])
```

---

## 7. Calculate Area of a Rectangle

Create an algorithm and flowchart to input length and width, calculate
the area (**Area = Length × Width**), and display the result.

### ✔ Pseudocode

```text
START
    INPUT length, width
    area = length * width
    PRINT area
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT length, width/]
    B --> C[area = length * width]
    C --> D[/PRINT area/]
    D --> E([END])
```

---

## 8. Determine Pass or Fail

Write the algorithm and draw the flowchart for a program that takes a
student's average marks and displays **"Pass"** if average ≥ 50,
otherwise **"Fail"**.

### ✔ Pseudocode

```text
START
    INPUT average_marks
    IF average_marks >= 50 THEN
        PRINT "Pass"
    ELSE
        PRINT "Fail"
    ENDIF
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT average_marks/]
    B --> C{average_marks >= 50 ?}
    C -->|Yes| D[/PRINT "Pass"/]
    C -->|No| E[/PRINT "Fail"/]
    D --> F([END])
    E --> F([END])
```

---

## 9. Calculate Factorial of a Number

Write the algorithm and draw the flowchart that input a number and
calculate its factorial using a loop.

---

## 10. Calculate Discount on Purchase

Write the algorithm and draw the flowchart for a program that inputs the
purchase amount and gives a **10% discount** if the amount is greater
than 1000.

### ✔ Pseudocode

```text
START
    INPUT purchase_amount
    discount_percent = 10
    IF purchase_amount > 1000 THEN
        purchase_amount -=  purchase_amount * discount_percent / 100
    ENDIF
    PRINT pirchase_amount
END
```

### ✔ Flowchart

```mermaid
flowchart TD
    A([START]) --> B[/INPUT purchase_amount/]
    B --> C{purchase_amount > 1000 ?}
    C -->|Yes| D[purchase_amount -= purchase_amount * 10 / 100]
    C -->|No| E[/PRINT purchase_amount/]
    D --> E[/PRINT purchase_amount/]
    E --> G([END])
```
---
