# 00a - Before We Begin (Prerequisites) 🧠

Before writing a single line of C code, there are a few core concepts and mindsets you need to understand. Programming is not just typing; it's a way of thinking.

## 1. The Programmer's Mindset
* **The Computer is Dumb:** A computer has zero common sense. It will do *exactly* what you tell it to do, even if it's completely wrong. 
* **Embrace Frustration:** You will get errors. You will spend 30 minutes looking for a missing semicolon. **This is completely normal.** Even professional engineers with 10 years of experience do this every day.
* **Break It Down:** Never try to solve a big problem all at once. Break it down into the smallest possible steps (this is called an *Algorithm*).

## 2. Files and Folders
You need to be comfortable with how files work on your computer.
* C code is just plain text. We save it in files ending with the `.c` extension (e.g., `main.c`).
* You must know exactly *where* you saved your file (the directory path) so you can tell the compiler where to find it.

## 3. Terminal / Command Line Survival
You will be using the black screen (Terminal/Command Prompt) to talk to the compiler. You only need to know a few commands:
* `pwd` (or `cd` with no arguments on Windows): **P**rint **W**orking **D**irectory. "Where am I right now?"
* `ls` (or `dir` on Windows): **L**i**s**t files. "What files are in this folder?"
* `cd folder_name`: **C**hange **D**irectory. "Open this folder."
* `cd ..`: "Go back out one folder."

## 4. The Text Editor
You can't write code in Microsoft Word. Word adds hidden formatting (fonts, colors, sizes) that confuses the compiler. You must use a pure text editor like **VS Code**, **Notepad++**, or even just plain **Notepad**.

## 5. Installing the C Compiler (GCC)
You can't compile C code without a compiler! Here is how you install GCC based on your OS:

* **Windows:** The easiest way is using [MSYS2](https://www.msys2.org/) or [Chocolatey](https://chocolatey.org/). If you have Chocolatey, open an Administrator PowerShell and run: `choco install mingw -y`.
* **Mac:** Open your Terminal and run: `xcode-select --install`. This installs the Apple developer tools (which includes the compiler).
* **Linux:** Open your terminal and run: `sudo apt install build-essential`.

> [!tip] Verification
> After installing, you must open a **brand new terminal window** (so it refreshes your PATH) and type `gcc --version`. If it prints out some version numbers, you are officially ready to code!

> [!info] Exercise / Tip
> Take a moment to practice navigating the terminal for 5 minutes. Create a folder, go into it, and check where they are. If you aren't comfortable in the terminal, compiling C code will feel like magic instead of logic.

➡️ Next: [01 Architecture and Compilation](01_Architecture_and_Compilation.md)
