# Libft Project

This project creates a C library, `libft.a`, containing a collection of general-purpose functions for use in future C programming assignments. It focuses on reimplementing standard C library functions, adding custom utility functions, and implementing linked list operations for enhanced functionality.

## Overview

### Objective
Develop a robust, reusable C library with essential functions for string, memory, and list manipulation, adhering to strict coding standards.

### Structure
- **Mandatory Part**: Includes reimplementations of standard C library functions and additional utility functions for string and memory operations.
- **Bonus Part**: Adds functions for manipulating singly linked lists using a `t_list` structure.

### Constraints
- Global variables are prohibited.
- Helper functions must be static to limit their scope.
- All files must be placed at the root of the repository.
- Must compile with `-Wall`, `-Wextra`, `-Werror` flags.
- No memory leaks allowed in user-written code.
- Library created using `ar`, not `libtool`.

## Features

### Mandatory Program (`libft.a`)
- **Part 1 - Libc Functions**: Reimplements standard C functions with `ft_` prefix, matching their original behavior (e.g., `ft_strlen`, `ft_memcpy`, `ft_strlcpy`, `ft_isalpha`, `ft_toupper`, etc.).
- **Part 2 - Additional Functions**:
 - `ft_substr`: Extracts a substring from a given string.
 - `ft_strjoin`: Concatenates two strings.
 - `ft_strtrim`: Trims specified characters from the start and end of a string.
 - `ft_split`: Splits a string into an array using a delimiter.
 - `ft_itoa`: Converts an integer to a string.
 - `ft_strmapi`: Applies a function to each character of a string, creating a new string.
 - `ft_striteri`: Applies a function to each character of a string in place.
 - `ft_putchar_fd`, `ft_putstr_fd`, `ft_putendl_fd`, `ft_putnbr_fd`: Outputs characters, strings, or integers to a file descriptor.

### Bonus Program
- Implements a singly linked list using the `t_list` structure with `content` (void *) and `next` (t_list *) members.
- **Bonus Functions**:
 - `ft_lstnew`: Creates a new list node with given content.
 - `ft_lstadd_front`: Adds a node to the front of the list.
 - `ft_lstsize`: Returns the number of nodes in the list.
 - `ft_lstlast`: Returns the last node of the list.
 - `ft_lstadd_back`: Adds a node to the end of the list.
 - `ft_lstdelone`: Frees a single nodes content, with a deletion function for cleanup.

## Technical Details

- **Language**: C
- **Allowed Functions**: `malloc`, `free`, `write` (specific to certain functions).
- **Files**: `Makefile`, `libft.h`, `ft_*.c`, bonus files as `ft_*_bonus.c`/`ft_*_bonus.h`.
- **Makefile**: Includes rules for `NAME`, `all`, `clean`, `fclean`, `re`, and `bonus` for the bonus part.
- **Directory Structure**: All files at the root of the repository.
- **Output**: Creates `libft.a` at the root using the `ar` command.

## Learning Outcomes

- Mastery of C function implementation and memory management.
- Understanding standard C library behaviors and their recreation.
- Experience with linked list manipulation and dynamic memory allocation.
- Building a reusable library for modular programming.
