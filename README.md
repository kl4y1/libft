# 📚 Libft

## 🧠 Overview

`libft` is a custom C library that reimplements essential functions from the standard C library, along with additional utility functions and linked list management.

This project is part of the 42 curriculum and serves as the foundation for all future C projects.

It focuses on mastering:
- Memory management
- Pointer manipulation
- String handling
- Linked lists
- Modular programming
- Defensive coding

---

# 📂 Project Structure

```
.
├── Makefile
├── libft.h
├── ft_*.c
├── libft-bonus/
│   ├── ft_lstadd_back_bonus.c
│   ├── ft_lstadd_front_bonus.c
│   ├── ft_lstclear_bonus.c
│   ├── ft_lstdelone_bonus.c
│   ├── ft_lstiter_bonus.c
│   ├── ft_lstlast_bonus.c
│   ├── ft_lstmap_bonus.c
│   ├── ft_lstnew_bonus.c
│   └── ft_lstsize_bonus.c
```

---

# 🚀 Compilation

Compile the mandatory part:

```bash
make
```

This generates:

```
libft.a
```

Compile with bonus:

```bash
make bonus
```

Clean object files:

```bash
make clean
```

Remove everything:

```bash
make fclean
```

Recompile:

```bash
make re
```

---

# 📦 Mandatory Functions

### 🔤 Character Classification

- `ft_isalpha`
- `ft_isdigit`
- `ft_isalnum`
- `ft_isascii`
- `ft_isprint`
- `ft_toupper`
- `ft_tolower`

---

### 🧵 String Functions

- `ft_strlen`
- `ft_strchr`
- `ft_strrchr`
- `ft_strncmp`
- `ft_strlcpy`
- `ft_strlcat`
- `ft_strdup`
- `ft_strnstr`
- `ft_substr`
- `ft_strjoin`
- `ft_strtrim`
- `ft_split`
- `ft_strmapi`
- `ft_striteri`

---

### 🧠 Memory Functions

- `ft_memset`
- `ft_bzero`
- `ft_memcpy`
- `ft_memmove`
- `ft_memchr`
- `ft_memcmp`
- `ft_calloc`

---

### 🔢 Conversion

- `ft_atoi`
- `ft_itoa`

---

### 📤 File Descriptor Output

- `ft_putchar_fd`
- `ft_putstr_fd`
- `ft_putendl_fd`
- `ft_putnbr_fd`

---

# ⭐ Bonus Part — Linked Lists

The bonus part implements a generic singly linked list.

## Structure

```c
typedef struct s_list
{
    void            *content;
    struct s_list   *next;
}   t_list;
```

## Linked List Functions

- `ft_lstnew`
- `ft_lstadd_front`
- `ft_lstsize`
- `ft_lstlast`
- `ft_lstadd_back`
- `ft_lstdelone`
- `ft_lstclear`
- `ft_lstiter`
- `ft_lstmap`

These functions allow:
- Creating nodes
- Adding/removing elements
- Iterating through the list
- Mapping a function over the list

---

# 🛠 Allowed Functions

Only the following standard functions are allowed:

- `malloc`
- `free`
- `write`

No usage of original libc equivalents for reimplemented functions.

---

# 🎯 Objectives

- Understand how libc functions work internally
- Improve pointer arithmetic skills
- Write memory-safe C code
- Handle edge cases (NULL, empty strings, overflow)
- Avoid memory leaks
- Create a reusable personal C library

---

# 🧪 Testing & Validation

Each function should be tested for:

- NULL inputs
- Empty strings
- Edge cases
- Memory leaks (using `valgrind`)
- Correct return values

Compilation flags:

```bash
-Wall -Wextra -Werror
```

---

# 🔗 Usage in Other Projects

To use `libft` in another project:

```bash
cc main.c -L. -lft
```

Or in your Makefile:

```make
LIBFT = libft/libft.a

$(NAME): $(OBJ)
	$(CC) $(CFLAGS) $(OBJ) $(LIBFT) -o $(NAME)
```

---

# 🏁 Final Result

`libft` is the foundation for future 42 projects such as:

- ft_printf
- get_next_line
- pipex
- minishell
- cub3d
- webserv

Mastering this project ensures strong fundamentals in C programming.


