# 📚 Libft — Custom C Library

> First project at 42 — Reimplementation of essential C standard library functions from scratch.

![Score](https://img.shields.io/badge/Score-125%2F100-brightgreen?style=flat-square)
![Language](https://img.shields.io/badge/Language-C-00599C?style=flat-square&logo=c&logoColor=white)
![School](https://img.shields.io/badge/School-42-000000?style=flat-square)

---

## 📌 Overview

`libft` is the very first project of the 42 curriculum. The goal is to build a personal C library by reimplementing over 40 functions from `<string.h>`, `<stdlib.h>`, `<ctype.h>` and more — without using the originals.

This library is then reused and extended throughout the entire 42 curriculum.

---

## ⚙️ Functions Implemented

**Libc functions**
| Function | Description |
|----------|-------------|
| `ft_memset` | Fill memory with a constant byte |
| `ft_bzero` | Zero a byte string |
| `ft_memcpy` | Copy memory area |
| `ft_memmove` | Copy memory area (handles overlap) |
| `ft_memchr` | Scan memory for a character |
| `ft_memcmp` | Compare memory areas |
| `ft_strlen` | Calculate string length |
| `ft_strdup` | Duplicate a string |
| `ft_strcpy` / `ft_strlcpy` | Copy a string |
| `ft_strcat` / `ft_strlcat` | Concatenate strings |
| `ft_strchr` / `ft_strrchr` | Locate character in string |
| `ft_strncmp` | Compare strings |
| `ft_strnstr` | Locate substring in string |
| `ft_atoi` | Convert string to integer |
| `ft_isalpha` / `ft_isdigit` / `ft_isalnum` | Character checks |
| `ft_isascii` / `ft_isprint` | More character checks |
| `ft_toupper` / `ft_tolower` | Character conversion |
| `ft_calloc` | Allocate zeroed memory |

**Additional functions**
| Function | Description |
|----------|-------------|
| `ft_substr` | Extract a substring |
| `ft_strjoin` | Join two strings |
| `ft_strtrim` | Trim characters from string edges |
| `ft_split` | Split string by delimiter |
| `ft_itoa` | Convert integer to string |
| `ft_strmapi` | Apply function to each char |
| `ft_striteri` | Apply function to each char (in-place) |
| `ft_putchar_fd` | Output a char to a file descriptor |
| `ft_putstr_fd` | Output a string to a file descriptor |
| `ft_putendl_fd` | Output a string + newline to fd |
| `ft_putnbr_fd` | Output an integer to a file descriptor |

**Bonus — Linked Lists**
| Function | Description |
|----------|-------------|
| `ft_lstnew` | Create a new list node |
| `ft_lstadd_front` | Add node at front |
| `ft_lstadd_back` | Add node at back |
| `ft_lstsize` | Count list nodes |
| `ft_lstlast` | Return last node |
| `ft_lstdelone` | Delete a node |
| `ft_lstclear` | Delete all nodes |
| `ft_lstiter` | Iterate over list |
| `ft_lstmap` | Map function over list |

---

## 🛠️ Usage

```bash
git clone https://github.com/Fazejli/libft.git
cd libft
make        # Compile the library
make bonus  # Compile with linked list functions
```

Then include it in your project:
```c
#include "libft.h"
```

And compile with:
```bash
gcc your_file.c -L. -lft -o your_program
```

---

## 📁 Project Structure

```
libft/
├── Makefile
├── libft.h
├── ft_*.c        # All function source files
└── ft_lst*.c     # Bonus linked list functions
```

---

## 🧠 Key Concepts

- Memory management in C (`malloc`, `free`)
- Pointer arithmetic
- String manipulation
- Linked list data structure
- Writing a static library with `ar`
- Makefile rules (`all`, `clean`, `fclean`, `re`, `bonus`)
