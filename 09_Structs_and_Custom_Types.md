# 09 - Structs (Custom Types) 🧱

What if you are making a video game and you need a Player? A player has a Name (text), a Score (integer), and Health (decimal). 
Instead of keeping track of three separate variables, we can glue them together into a **Struct**.

## Creating a Struct
A struct is like creating your very own custom Data Type (like your own custom box).

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
    // 2. Create an actual player using the blueprint
    struct Player p1;
    
    // 3. Use the DOT (.) to access their specific stats
    p1.score = 100;
    p1.health = 95.5;
    strcpy(p1.name, "Hero"); // Copies the word "Hero" into the name array
    
    printf("%s has %d points!\n", p1.name, p1.score);
    
    return 0;
}
```

### 🎉 Congratulations!
You've made it through the core logic of C programming! You understand memory, pointers, loops, and logic. You are well on your way to becoming a real programmer. Keep practicing, and don't be afraid to break things!

⬅️ Back: [08 Arrays and Strings](08_Arrays_and_Strings.md)
