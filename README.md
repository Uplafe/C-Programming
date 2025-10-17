# 🧠 C Programming Projects — First Year Computer Science

Welcome to my C programming showcase!  
This repository contains all the programs I’ve written as part of my first-year CS journey.  
Each section below includes:
- The **program title**
- The **source code** (embedded)
- A **screenshot/output image**

---

## 📂 Table of Contents

1. [Simple Calculator](#-simple-calculator)
2. [Individual Arithmetic Operations Calculator](#-individual-arithmetic-operations-calculator)
3. [Even Or Odd Identifier](#-even-or-odd-identifier)
4. [Alphabets Vowel Checker](#-alphabets-vowel-checker)
5. [Age Verification](#-age-verification)
6. [Simple Interest Calculator](#-simple-interest-calculator)
7. [Largest of Two Numbers](#-largest-of-two-numbers)
8. [Swap Two Numbers](#-swap-two-numbers)
9. [Positive, Negative, or Zero](#️-positive-negative-or-zero)
10. [Shopping Discount System](#-shopping-discount-system)

---

## 🧮 Simple Calculator

**Description:**  
A program that allows users to calculate simple equations.

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

### ➕ Addition
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

### ✖️ Multiplication
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

### ➗ Division
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
### 🔁 Combined Calculator (All Operations)
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
## 🔢 Even or Odd Identifier

**Description:** 
A program that allows users to identify if a value is even or odd.
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
### 🌀 Even or Odd Identifier using (goto) Statement
#include <stdio.h>
```c
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
```
## 🔠 Alphabets Vowel Checker

**Description:** 
A program that allows users to identify if a character is a vowel or consonant.
```c
#include <stdio.h>

int main() 
{
    char c;
    printf("Enter a character: ");
    scanf(" %c", &c); 
    
    if (c == 'a' || c == 'e' || c == 'i' || c == 'o' || c == 'u' ||
        c == 'A' || c == 'E' || c == 'I' || c == 'O' || c == 'U')
    {
        printf("The character is a vowel.\n");  
    }
    else
    {
        printf("The character is a consonant.\n");
    }

    return 0;
}
```
## 🔞 Age Verification

**Description:** 
A program that allows users to identify if the inputted age is eligible or underage.
```c
#include <stdio.h>

int main() 
{
    int age;
    
    printf("Enter your age: ");
    scanf("%d", &age);

    if (age >= 18) {
        printf("You are eligible");
    } 
    else {
        printf("You are under 18.\n");
    }

    return 0;
}
```
## 💹 Simple Interest Calculator

**Description:** 
A program that allows users to calculate simple interest.
```c
#include <stdio.h>

int main() 
{
    int p, t;     
    float r, z;     

    printf("Input principal: ");
    scanf("%d", &p);

    printf("Input interest rate: ");
    scanf("%f", &r);

    printf("Input time in months: ");
    scanf("%d", &t);

    z = (p * r * t) / 100;

    printf("Your total interest is: %.2f\n", z);

    return 0;
}
```
## 🟰 Largest of Two Numbers

**Description:** 
A program that allows users to find the greatest of two values.
```c
#include <stdio.h>

int main() 
{
    int a, b;

    printf("Enter first number: ");
    scanf("%d", &a);

    printf("Enter second number: ");
    scanf("%d", &b);

    if (a > b) {
        printf("%d is the largest number.\n", a);
    } 
    else if (b > a) {
        printf("%d is the largest number.\n", b);
    } 
    else {
        printf("Both numbers are equal.\n");
    }

    return 0;
}
```
## 🔁 Swap Two Numbers

**Description:** 
Demonstrates variable swapping using a temporary variable.
```c
#include <stdio.h>

int main() 
{
    int a, b, temp;

    printf("Enter first number: ");
    scanf("%d", &a);

    printf("Enter second number: ");
    scanf("%d", &b);

    temp = a;
    a = b;
    b = temp;

    printf("After swapping:\n");
    printf("First number = %d\n", a);
    printf("Second number = %d\n", b);

    return 0;
}
```
## ⚖️ Positive, Negative, or Zero

**Description:** 
Checks if a number is positive, negative, or zero.
```c
#include <stdio.h>

int main() 
{
    int num;

    printf("Enter a number: ");
    scanf("%d", &num);

    if (num > 0) {
        printf("The number is positive.\n");
    } 
    else if (num < 0) {
        printf("The number is negative.\n");
    } 
    else {
        printf("The number is zero.\n");
    }

    return 0;
}
```
## 🏷️ Shopping Discount System

**Description:**
This program calculates the total bill amount after applying membership-based discounts.
```c
#include <stdio.h>

int main() 
{
int mem;
float bill;
 printf("Memberships: \n 1. Gold, \n 2. Silver, \n 3. Not a Member \n Select a membership to continue:");
   scanf("%d",&mem);
 printf("Enter billing amount:");
   scanf("%f",&bill);
switch (mem)
{
   case 1:
   {
   if(bill>=500)
   printf("Gold Member - Total: %f", bill - (20*bill/100));
   else
   printf("Gold Member - Total: %f", bill);
   }
   break;
   
   case 2:
   {
   if(bill>=500)
   printf("Silever Member - Total: %f", bill - (10*bill/100));
   else
   printf("Silever Member - Total: %f", bill);
   }
   break;
   
   case 3:
   {
   if(bill>=500)
   printf("No Membership - Total: %f", bill - (5*bill/100));
   else
   printf("No Membership - Total: %f", bill);
   }
   break;
}
return 0;
}
```
## 🚦 Traffic Light Signal System

**Description:**
A simple traffic light simulation that instructs users what action to take depending on the traffic signal color they choose.
```c
#include <stdio.h>

int main() {
    int signal;

    printf("Traffic Signal: \n 1. Green (Go) \n 2. Yellow (Ready to stop) \n 3. Red (Stop)\n");
    printf("Enter your choice (1-3): ");
    scanf("%d", &signal);

    switch(signal) {
        case 1:
            printf("GO\n");
            break;

        case 2:
            printf("Ready to Stop\n");
            break;

        case 3:
            printf("Stop\n");
            break;

        default:
            printf("Invalid input\n");
    }

    return 0;
}
```
