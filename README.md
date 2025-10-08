# 🧩 Libft

A custom C library that recreates standard C library functions and adds new utility functions.  
This project is part of the 42 curriculum and serves as a foundation for future projects.

---

## 📘 Overview

The **libft** project aims to rebuild essential functions from the C standard library,  
as well as create additional functions for memory management, strings, linked lists, and more.  

You’ll end up with your own personal C library that you can reuse in future 42 projects.

---

## 🛠️ Compilation

To compile the library:
```bash
    make

To remove object files:
    make clean

To remove all generated files (including libft.a):
    make fclean

To rebuild everything:
    make re

🧩 Example Usage

    #include "libft.h"
    #include <stdio.h>

    int main(void)
    {
        char str[] = "Hello, World!";
        printf("Length: %zu\n", ft_strlen(str));
        return (0);
    }

Compile and run:
    cc main.c -L. -lft && ./a.out

🧑‍💻 Author

    . Abdullah Sauafth
    📧 [jabr.abood@yahoo.com]