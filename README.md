# 🧩 Libft

<div align="center">

![42 School](https://img.shields.io/badge/42-School-000000?style=for-the-badge&logo=42&logoColor=white)
![C](https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-yellow.svg?style=for-the-badge)

**A custom C library recreating standard library functions**  
*Part of the 42 School curriculum*

</div>

---

## 📖 About

**Libft** is a comprehensive C library that reimplements essential functions from the standard C library, along with additional utility functions for enhanced functionality. This project serves as the foundation for all future 42 School projects.

### ✨ Key Features

- **Standard Library Functions**: Recreated from scratch
- **Memory Management**: Safe and efficient memory operations
- **String Manipulation**: Comprehensive string handling utilities
- **Input/Output**: File descriptor operations
- **Type Conversion**: Robust conversion functions

---

## 📘 Overview

The **libft** project aims to rebuild essential functions from the C standard library,  
as well as create additional functions for memory management, strings, linked lists, and more.  

You’ll end up with your own personal C library that you can reuse in future 42 projects.

---

## � Quick Start

### Prerequisites
- GCC compiler
- Make utility
- Linux/macOS environment

### 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/aboodjabr0/libft.git
   cd libft
   ```

2. **Compile the library**
   ```bash
   make
   ```

### 🛠️ Build Commands

| Command | Description |
|---------|-------------|
| `make` | Compile the library |
| `make clean` | Remove object files |
| `make fclean` | Remove all generated files |
| `make re` | Rebuild everything |

---

## 💡 Usage Example

```c
#include "libft.h"
#include <stdio.h>

int main(void)
{
    // String manipulation
    char *str = "Hello, World!";
    printf("Original: %s\n", str);
    printf("Length: %zu\n", ft_strlen(str));
    printf("Uppercase: %s\n", ft_strmapi(str, (char (*)(unsigned int, char))ft_toupper));
    
    // Memory operations
    char *dup = ft_strdup(str);
    printf("Duplicate: %s\n", dup);
    
    // String splitting
    char **words = ft_split("apple,banana,orange", ',');
    for (int i = 0; words[i]; i++)
        printf("Word %d: %s\n", i + 1, words[i]);
    
    return (0);
}
```

**Compile and run:**
```bash
cc example.c -L. -lft -o example && ./example
```

---

## 📚 Function Categories

<details>
<summary><strong>🔤 Character Functions</strong></summary>

- `ft_isalpha()` - Check if character is alphabetic
- `ft_isdigit()` - Check if character is digit
- `ft_isalnum()` - Check if character is alphanumeric
- `ft_isascii()` - Check if character is ASCII
- `ft_isprint()` - Check if character is printable
- `ft_toupper()` - Convert to uppercase
- `ft_tolower()` - Convert to lowercase

</details>

<details>
<summary><strong>📝 String Functions</strong></summary>

- `ft_strlen()` - Calculate string length
- `ft_strchr()` - Find character in string
- `ft_strrchr()` - Find last occurrence of character
- `ft_strncmp()` - Compare strings (n characters)
- `ft_strlcpy()` - Safe string copy
- `ft_strlcat()` - Safe string concatenation
- `ft_strnstr()` - Find substring (n characters)
- `ft_strdup()` - Duplicate string
- `ft_substr()` - Extract substring
- `ft_strjoin()` - Join strings
- `ft_strtrim()` - Trim string
- `ft_split()` - Split string by delimiter
- `ft_strmapi()` - Apply function to each character
- `ft_striteri()` - Apply function to each character with index

</details>

<details>
<summary><strong>🧠 Memory Functions</strong></summary>

- `ft_memset()` - Fill memory with byte
- `ft_bzero()` - Zero out memory
- `ft_memcpy()` - Copy memory
- `ft_memmove()` - Safe memory move
- `ft_memchr()` - Find byte in memory
- `ft_memcmp()` - Compare memory blocks
- `ft_calloc()` - Allocate and zero memory

</details>

<details>
<summary><strong>🔄 Conversion Functions</strong></summary>

- `ft_atoi()` - String to integer
- `ft_itoa()` - Integer to string

</details>

<details>
<summary><strong>📤 Output Functions</strong></summary>

- `ft_putchar_fd()` - Output character to file descriptor
- `ft_putstr_fd()` - Output string to file descriptor
- `ft_putendl_fd()` - Output string with newline to file descriptor
- `ft_putnbr_fd()` - Output number to file descriptor

</details>

---

## 🎯 Learning Objectives

- Understanding **memory management** in C
- Implementing **low-level functions** from scratch
- Working with **pointers** and **arrays**
- **File descriptor** operations
- **Makefile** creation and management
- **Code organization** and documentation

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Abdullah Sauafth**
- 📧 Email: [jabr.abood@yahoo.com](mailto:jabr.abood@yahoo.com)
- 🐙 GitHub: [@aboodjabr0](https://github.com/aboodjabr0)
- 🏫 42 School Student

---

<div align="center">

**⭐ Star this repository if you found it helpful!**

Made with ❤️ at 42 School

</div>