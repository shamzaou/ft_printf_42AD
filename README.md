# ft_printf

ft_printf is a custom implementation of the standard C library function `printf`. This project is written in C and serves as a reliable and efficient alternative to the built-in `printf` function. The implementation aims to match the functionality of the original `printf` while adhering to strict coding standards.

## Features

ft_printf supports the following format specifiers:

- `%c`: Character
- `%s`: String
- `%p`: Pointer address
- `%d`: Signed decimal integer
- `%i`: Signed decimal integer
- `%u`: Unsigned decimal integer
- `%x`: Unsigned hexadecimal integer (lowercase)
- `%X`: Unsigned hexadecimal integer (uppercase)
- `%%`: Literal '%' character

## Usage

To use ft_printf in your project, follow these steps:

1. Clone the ft_printf repository:
   ```
   git clone https://github.com/shamzaou/ft_printf_42AD.git
   ```

2. Compile the ft_printf library:
   ```
   cd ft_printf
   make
   ```

3. Include the `ft_printf.h` header file in your C source files:
   ```c
   #include "ft_printf.h"
   ```

4. Link the `libftprintf.a` library file when compiling your project:
   ```
   gcc -L. -lftprintf your_source_files.c
   ```

5. Use `ft_printf` in your code as you would use the standard `printf` function:
   ```c
   ft_printf("Hello, %s!\n", "world");
   ```

## Example

Here's a simple example that demonstrates the usage of ft_printf:

```c
#include "ft_printf.h"

int main()
{
    int a = 42;
    char *str = "ft_printf";

    ft_printf("Hello, %s!\n", "world");
    ft_printf("This is an example of using %s.\n", str);
    ft_printf("The answer to life, the universe, and everything is %d.\n", a);
    ft_printf("The memory address of the variable 'a' is %p.\n", &a);

    return 0;
}
```

## Conclusion

Implementing ft_printf is a valuable exercice for coders looking to enhance their C programming skils.
