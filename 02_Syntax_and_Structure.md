# 02 - Your First Program 🏗️

Let's look at the classic "Hello World" program. This is the absolute minimum code you need.

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

## Breaking it down line-by-line

### 1. `#include <stdio.h>`
Think of this as going to the library to borrow a dictionary. `stdio.h` stands for **St**andar**d** **I**nput **O**utput. It gives our program the ability to print text to the screen!

### 2. `int main()`
This is the **front door** of your house. Whenever the computer runs your program, it searches for `main()` and starts reading from there. 

### 3. `{ ... }` (Curly Braces)
These group code together. Everything inside these braces is a set of instructions that belongs to the `main` function.

### 4. `printf("Hello, World!\n");`
* `printf` means "print formatted text".
* `\n` is a secret code that means "Press the Enter key" (New line).
* **Crucial Rule:** Every instruction in C **MUST** end with a semicolon `;`. It is the period at the end of a sentence. If you forget it, the compiler will panic.

### 5. `return 0;`
This tells the computer "The program finished successfully with 0 errors!"

➡️ Next: [03 Data Types and Memory](03_Data_Types_and_Memory.md)
⬅️ Back: [01 Architecture and Compilation](01_Architecture_and_Compilation.md)
