# 09 - Structs and Custom Types 🧱

What if we want to group an `int` (age), a `float` (height), and a `char array` (name) together? We use a `struct`.

## Defining and Using a Struct

```c
#include <stdio.h>
#include <string.h>

// 1. Define the blueprint
struct Player {
    char name[50];
    int score;
    float health;
};

int main() {
    // 2. Create an instance (allocates memory for all 3 things back-to-back)
    struct Player p1;
    
    // 3. Use the DOT operator to access members
    p1.score = 100;
    p1.health = 95.5;
    strcpy(p1.name, "Hero"); // Must use strcpy for string arrays!
    
    printf("%s has %d points.", p1.name, p1.score);
    return 0;
}
```

## Pointers to Structs (The Arrow Operator)
When you have a pointer to a struct, using `(*p).score` is ugly. C gives us the Arrow Operator `->` as a shortcut.

```c
struct Player *ptr = &p1;
ptr->score = 200; // Exact same as (*ptr).score = 200;
```

> [!tip] Deep Dive: Memory Alignment and Padding
> You might think the size of `struct Player` is `50 (name) + 4 (score) + 4 (health) = 58 bytes`. 
> However, `sizeof(struct Player)` might return `60`. Why? 
> CPUs read memory in chunks (e.g., 4 or 8 bytes at a time). The compiler injects "Padding" (empty, unused bytes) between struct members to align them to boundaries so the CPU can read them faster. 

---
### 🎓 Course Complete!
You now have the fundamental and underlying architectural knowledge to write C like an absolute pro. Good luck!
