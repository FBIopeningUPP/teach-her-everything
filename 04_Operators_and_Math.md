# 04 - Operators and Math 🧮

C gives you various tools to manipulate data in memory.

## 1. Arithmetic Operators
`+`, `-`, `*`, `/`, `%` (Modulo - remainder of division).
* **Deep Dive on Division:** If you divide two integers (e.g., `5 / 2`), C performs **Integer Division** and truncates the decimal. The result is `2`, not `2.5`. To get decimals, at least one number must be a float (`5.0 / 2`).

## 2. Relational & Logical Operators
* `==`, `!=`, `>`, `<`, `>=`, `<=`
* `&&` (Logical AND), `||` (Logical OR), `!` (Logical NOT)
* **Short-circuiting (Deep Dive):** In `if (A && B)`, if `A` is false, C doesn't even evaluate `B` because the whole thing is already guaranteed false.

## 3. Bitwise Operators (For the Curious)
These manipulate the raw 1s and 0s in memory. Highly used in embedded systems.
* `&` (Bitwise AND)
* `|` (Bitwise OR)
* `^` (Bitwise XOR)
* `~` (Bitwise NOT / One's complement)
* `<<` (Left Shift - multiplies by powers of 2)
* `>>` (Right Shift - divides by powers of 2)

```c
int a = 5;      // Binary: 0101
int b = a << 1; // Shifts bits left by 1: 1010 (which is 10 in decimal)
```

## 4. Increment/Decrement
`x++` (Post-increment) vs `++x` (Pre-increment).
* `x++`: Use the current value of `x`, THEN add 1.
* `++x`: Add 1 to `x` FIRST, then use the new value.

➡️ Next: [[05_Control_Flow_and_Loops]]
