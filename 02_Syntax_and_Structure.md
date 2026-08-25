# 02 - Syntax and Structure 🏗️

Let's break down the classic Hello World program line-by-line.

```c
#include <stdio.h>

int main(int argc, char *argv[]) {
    printf("Hello, World!\n");
    return 0;
}
```

## Line-by-Line Breakdown

### 1. `#include <stdio.h>`
* **Beginner:** "We are borrowing the Standard Input/Output dictionary from the library so we know how to print words."
* **Nerd Note:** The angle brackets `< >` tell the preprocessor to look in the system's default include directories (like `/usr/include`). If you used quotes `"myheader.h"`, it looks in the current directory first.

### 2. `int main(int argc, char *argv[])`
* **Beginner:** This is the main door to your house. The OS always starts running the program here.
* **Nerd Note:** 
  * `int`: The function returns an integer to the Operating System. `0` means success, anything else (like `1` or `-1`) means an error occurred.
  * `argc` (Argument Count): The number of command-line arguments passed to the program.
  * `argv` (Argument Vector): An array of strings containing the arguments. (e.g., `./program arg1` -> `argc` is 2, `argv[0]` is "./program", `argv[1]` is "arg1").

### 3. `{ ... }`
These define a **Block** or **Scope**. Everything inside belongs to `main`.

### 4. `printf("Hello, World!\n");`
* Prints formatted string. `\n` is an escape sequence representing the newline character (ASCII 10).
* **Crucial:** Semicolons `;` are statement terminators. They tell the compiler "this instruction is over."

➡️ Next: [[03_Data_Types_and_Memory]]
