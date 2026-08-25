# 07 - Pointers Demystified 🎯

**This is where C separates the pros from the noobs.** Take your time learning this.

## The Concept
A pointer is simply a variable that stores a **memory address** instead of a normal value.

> [!info] Helpful Analogy
> If a variable is a house with a family inside, a Pointer is a piece of paper with the house's address written on it (e.g., "123 Main St"). 

## The Two Operators
1. `&` (Address-of): "Where do you live?" Gets the memory address of a variable.
2. `*` (Dereference): "Go to the address and get what's inside."

```c
int age = 25;       // A variable storing 25
int *pAge = &age;   // pAge is a pointer storing the ADDRESS of age.

// Let's break down the * operator
printf("Value of age: %d\n", age);         // 25
printf("Address of age: %p\n", &age);      // e.g., 0x7ffd5342 (Memory Address)
printf("Value inside pAge: %p\n", pAge);   // 0x7ffd5342 (Memory Address)
printf("Value POINTED TO: %d\n", *pAge);   // 25 (Goes to the address and gets the value!)
```

## Simulating Pass by Reference
Now we can fix the problem from Chapter 6! We pass the address instead of a copy.

```c
// We accept a POINTER (an address)
void actuallyChange(int *x) {
    *x = 99; // Go to the address and change the value there to 99
}

int main() {
    int myNum = 5;
    actuallyChange(&myNum); // Pass the ADDRESS of myNum
    printf("%d", myNum);    // Prints 99!
    return 0;
}
```

> [!tip] Deep Dive: Pointer Arithmetic
> Pointers know the size of the data type they point to. If `int *p` points to address `1000`, doing `p++` will make it point to `1004` (since an `int` is 4 bytes). It jumps exactly one `int` forward in memory!

➡️ Next: [[08_Arrays_and_Strings]]
