# 03 - Data Types and Memory 💾

To master C, you must master Memory. 

## What is RAM, physically?
Imagine RAM as a giant street with billions of mailboxes. 
* Every mailbox can hold exactly **1 Byte** (8 Bits, e.g., `01001101`).
* Every mailbox has a unique address (e.g., Mailbox #1004).

## Data Types (The Size of the Box)
When you create a variable, C reserves mailboxes for you. Different types need different numbers of mailboxes.

| Type | Typical Size | Description | Example |
| :--- | :--- | :--- | :--- |
| `char` | 1 Byte | A single ASCII character. | `char grade = 'A';` |
| `int` | 4 Bytes | A whole number. | `int age = 25;` |
| `float` | 4 Bytes | Decimal number (single precision). | `float pi = 3.14f;` |
| `double`| 8 Bytes | Decimal number (double precision).| `double precise = 3.14159;` |

> [!info] Exercise / Tip: ASCII
> It is important to understand that computers don't know what 'A' is. They only know numbers. A `char` is just an integer (usually from 0 to 127). The letter 'A' is just the number `65` in disguise. 'B' is `66`, 'a' is `97`, etc.

```c
#include <stdio.h>
int main() {
    char letter = 'A';
    printf("As character: %c\n", letter); // Prints 'A'
    printf("As integer: %d\n", letter);   // Prints 65
    return 0;
}
```

> [!tip] Deep Dive: Signed vs Unsigned
> By default, `int` and `char` are signed (can be negative). One bit is used as the "sign bit" (Two's Complement). 
> - A signed `char` ranges from `-128` to `127`.
> - An `unsigned char` uses all 8 bits for positive numbers, ranging from `0` to `255`. 
> - You can check exact sizes on your machine using `sizeof(int)`.

➡️ Next: [[04_Operators_and_Math]]
