# 🧠 C Programming Projects — First Year Computer Science

Welcome to my C programming showcase!  
This repository contains all the programs I’ve written as part of my first-year CS journey.  
Each section below includes:
- The **program title**
- The **source code** (embedded)
- A **screenshot/output image**

---

## 📂 Table of Contents

1. [Shopping Discount System](#shopping-discount-system)
2. [Largest of Two Numbers](#largest-of-two-numbers)
3. [Swap Two Numbers](#swap-two-numbers)
4. [Positive, Negative, or Zero](#positive-negative-or-zero)
5. [Simple Interest Calculator](#simple-interest-calculator)

---

## 🛒 Shopping Discount System

**Description:**  
A program that calculates discounts based on membership type and total purchase.

### 💻 Code
```c
#include <stdio.h>

int main() {
    char member;
    float amount, discount = 0.0;

    printf("Enter membership type (G for Gold, S for Silver, N for None): ");
    scanf(" %c", &member);
    printf("Enter total purchase amount: ");
    scanf("%f", &amount);

    if (member == 'G' && amount > 500)
        discount = amount * 0.2;
    else if (member == 'S' && amount > 300)
        discount = amount * 0.1;

    printf("Discount: %.2f\n", discount);
    printf("Final amount: %.2f\n", amount - discount);

    return 0;
}
