# 03 - Data Types and Memory 💾

Programs need to remember things (like a player's health, a score, or a name). We use **Variables** for this.

## What is a Variable?
Imagine RAM (the computer's memory) as a massive wall of physical mailboxes. 
When you create a "variable," you are asking the computer to reserve a mailbox for you and slap a name-tag on it.

However, in C, you have to tell the computer **what kind of box** it is. You can't put a word in a box meant for a number!

## The 3 Main Boxes (Data Types)

| Type | What it holds | Example |
| :--- | :--- | :--- |
| `int` | Whole numbers (Integers) | `int age = 25;` |
| `float` | Decimal numbers | `float price = 19.99;` |
| `char` | A single letter/symbol | `char grade = 'A';` |

## Writing and Reading Variables

```c
#include <stdio.h>

int main() {
    // 1. Create a box for an integer called "score"
    int score;
    
    // 2. Put the number 100 inside the box
    score = 100;
    
    // 3. Print it. The %d is a special placeholder for integers!
    printf("My score is %d\n", score);
    
    return 0;
}
```

> [!tip] Placeholders for Printing
> When using `printf`, you use `%d` to print an `int`, `%f` to print a `float`, and `%c` to print a `char`.

➡️ Next: [04 Operators and Math](04_Operators_and_Math.md)
⬅️ Back: [02 Syntax and Structure](02_Syntax_and_Structure.md)
