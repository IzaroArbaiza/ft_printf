# 🖨️ ft_printf

`ft_printf` is a custom implementation of the C standard library function `printf`, developed as part of the core curriculum at [42 School](https://42.fr/en/homepage/).
It aims to reproduce the behavior of `printf`, handling formatted output with variable arguments, all written from scratch in C without relying on the standard `printf` function.


## 🔧 Overview
- Language: **C**  
- Norme compliant (42 coding style rules)  
- Manual handling of variable argument lists (`stdarg.h`)

### Key Concepts Practiced
- Variadic functions using `va_start`, `va_arg`, and `va_end`  
- Parsing and interpreting format strings  
- Handling multiple data types and flags  
- Custom number and string conversions  
- Low-level output using `write()`  
- Memory and buffer management

<br>

## 📋 Supported Format Specifiers
`ft_printf` supports the following format specifiers:
- `%c` — Character  
- `%s` — String  
- `%p` — Pointer address  
- `%d` / `%i` — Signed integers  
- `%u` — Unsigned integers  
- `%x` — Lowercase hexadecimal  
- `%X` — Uppercase hexadecimal  
- `%%` — Literal percent sign

<br>

## 📦🚀 How to Use
Clone the repository
```bash
git clone https://github.com/yourusername/ft_printf.git ft_printf
```
Get into the folder and compile it with Makefile
```bash
cd ft_printf && make
```

### 👉🏼 Usage
```C
#include "ft_printf.h"
```
and then don't forget to compile against the library
```Bash
gcc your_file.c libftprintf.a -I. && ./a.out
```
example:
```C
ft_printf("Hello %s, number is %+05d and hex %#x\n", "world", 42, 255);
```
