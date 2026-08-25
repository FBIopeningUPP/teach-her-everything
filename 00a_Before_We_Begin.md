# 00a - Before We Begin 🧠

Before writing a single line of code, you need to understand the "Programmer's Mindset." 

## 1. The Computer is Extremely Literal
Imagine a robot that makes sandwiches. If you tell it "Put peanut butter on bread", it might put the entire plastic jar on top of the bread bag. You have to tell it: "Open the bag. Take out one slice. Open the jar. Get a knife..."
**Computers are just like that robot. They have zero common sense.** If your code doesn't work, it's because the computer is doing *exactly* what you told it to do.

## 2. Embrace the Frustration
You will get errors. You will spend 20 minutes looking for a missing semicolon `;`. **This is completely normal.** Every professional programmer goes through this every single day. Errors are just the computer saying "I don't understand," not "You are bad at this."

## 3. The Terminal (The Black Screen)
You will use the "Terminal" (or Command Prompt) to talk to the computer without a mouse. 
* `pwd` (or `cd` on Windows): "Where am I?"
* `ls` (or `dir` on Windows): "What files are in this folder?"
* `cd folder_name`: "Open this folder."

## 4. Installing the Compiler
To write C, you need a "Compiler" (we'll explain what this is in the next chapter). We use **GCC**.
* **Windows:** Open an Administrator PowerShell and type: `choco install mingw -y`
* **Mac:** Open Terminal and type: `xcode-select --install`
* **Linux:** Open Terminal and type: `sudo apt install build-essential`

> [!tip] Verification
> Open a **brand new terminal window** and type `gcc --version`. If it prints out numbers, you are officially ready!

➡️ Next: [01 Architecture and Compilation](01_Architecture_and_Compilation.md)
⬅️ Back: [README](README.md)
