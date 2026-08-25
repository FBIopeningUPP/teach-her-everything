# 04 - Math and Logic 🧮

Computers are essentially just giant calculators. Here is how we do math.

## 1. Basic Math
You have your standard operators: `+` (add), `-` (subtract), `*` (multiply), `/` (divide).

```c
int a = 10;
int b = 3;
int total = a + b; // total is now 13
```

> [!tip] Deep Dive: The Weirdness of Division
> If you divide two integers in C (like `10 / 3`), the computer cuts off the decimal entirely! The answer will be `3`, not `3.33`. To get a decimal, you must use `float` boxes instead of `int` boxes.

## 2. The Remainder (Modulo)
The `%` operator gives you the **remainder** of division. It is incredibly useful!
`10 % 3` equals `1` (Because 3 goes into 10 three times, leaving 1 leftover). 

## 3. Asking Questions (Logic)
We often need to compare things.
* `>` (Greater than), `<` (Less than)
* `>=` (Greater than or equal to), `<=` (Less than or equal to)
* `==` (Exactly equal to) -> **Warning! Use two equals signs to compare! One equals sign `=` means "put this in the box".**
* `!=` (Not equal to)

## 4. Shortcuts
Programmers are lazy. Instead of writing `score = score + 1;`, we use a shortcut:
`score++;` (This means "Add 1 to score").

➡️ Next: [05 Control Flow and Loops](05_Control_Flow_and_Loops.md)
⬅️ Back: [03 Data Types and Memory](03_Data_Types_and_Memory.md)
