# C Programming Projects — First Year Computer Science

Welcome to my C programming showcase!  
This repository contains all the programs I’ve written as part of my first-year CS journey.  
Each section below includes:
- The **program title**
- The **source code** (embedded)
- A **screenshot/output image**

---

## 📂 Table of Contents

1. [Simple Calculator](#Simple-Calculator) Addition, Subtraction, Multiplication Calculator.
1. [Individual Arithmetic Operations Calculator ](#Individual_Arithmetic_Operations_Calculator)
2. [Even Or Odd Identifier](#Even_Or_Odd_Identifier)
3. [Swap Two Numbers](#swap-two-numbers)
4. [Positive, Negative, or Zero](#positive-negative-or-zero)
5. [Simple Interest Calculator](#simple-interest-calculator)

---

## 🧮 Simple Calculator

**Description:**  
A program that allows users to calculate simple equations.

### 💻 Code
```c
#include <stdio.h>

int main() 
{
int a, b;
int op_choice;
 printf("Enter 1 for Addition, 2 for Subtraction, 3 for Multiplication:");
  scanf("%d", &op_choice);
 switch (op_choice)
 {
     case 1:
      printf("Input the value of a(a+b=?):");
       scanf("%d",&a);
      printf("Input the value of b (a+b=?):");
       scanf("%d",&b);
      printf("The sum of %d and %d is %d",a,b,a+b);
      break;

     case 2:
      printf("Input the value of a(a-b=?):");
       scanf("%d",&a);
      printf("Input the value of b (a-b=?):");
       scanf("%d",&b);
      printf("The sum of %d and %d is %d",a,b,a-b);
      break;

     case 3:
      printf("Input the value of a(a x b=?):");
       scanf("%d",&a);
      printf("Input the value of b (a x b=?):");
       scanf("%d",&b);
      printf("The sum of %d and %d is %d",a,b,a*b);
      break;
      
     default:
     
     printf("Error");
 }
 
    return 0;
}

```

## 🧮 Individual Arithmetic Operations Calculator

**Description:**  
A program that allows users to calculate simple equations.

### 💻 Code

## ➕ Addition
```c

#include <stdio.h>

int main() {
    int a, b, sub; 
    printf("Enter the first value: "); 
    scanf("%d", &a); 
    printf("Enter the second value: "); 
    scanf("%d", &b); 
    sub = a - b;
    printf("The sub of %d and %d is %d\n", a, b, sub); 
    return 0;
}
```
## ✖️ Multiplication
```c
#include <stdio.h>

int main() {
    int a, b, mul; 
    printf("Enter the first value: "); 
    scanf("%d", &a); 
    printf("Enter the second value: "); 
    scanf("%d", &b); 
    mul = a * b;
    printf("The mul of %d and %d is %d\n", a, b, mul); 
    return 0;
}
```
## ➗ Division
```c
#include <stdio.h>

int main() {
    int a, b, div; 
    printf("Enter the first value: "); 
    scanf("%d", &a); 
    printf("Enter the second value: "); 
    scanf("%d", &b); 
   div = a / b;
    printf("The div of %d and %d is %d\n", a, b, div); 
    return 0;
}
```
## 🔁 Calculator combinded with all the previous operations.
```c
#include <stdio.h>

int main() {
    int a, b, sum, sub, mul, div;

    printf("Enter the first value: ");
    scanf("%d", &a);

    printf("Enter the second value: ");
    scanf("%d", &b);
    sum = a + b;
    printf("The sum of %d and %d is %d\n", a, b, sum);
    sub = a - b;
    printf("The subtraction of %d and %d is %d\n", a, b, sub);
    mul = a * b;
    printf("The multiplication of %d and %d is %d\n", a, b, mul);
    if (b != 0) {
        div = a / b;
        printf("The division of %d and %d is %d\n", a, b, div);
    } else {
        printf("Error: Division by zero is not allowed.\n");
    }

    return 0;
}
```
## 🧮 Even or Odd Identifier
**Description:**  
A program that allows users to identifiy if a value is even or odd.

```c
#include <stdio.h>

int main() {
    int a;
    printf("Enter the value: ");
    scanf("%d", &a);
    if (a % 2 == 0) { 
        printf("number is even"); 
    } else {
        printf("number is odd");
    }
    return 0;
}


```
# 🧮 Even or Odd Identifier using (goto) Statement
```C
#include <stdio.h>

int main() {
    int a;
    Here:
    printf("Enter the value: ");
    scanf("%d", &a);
    if (a % 2 == 0) { 
        printf("number is even\n");
    } else {
        printf("number is odd\n");
    }
    
    
 goto Here;
 return 0;
} 
```c
