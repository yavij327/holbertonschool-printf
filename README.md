# _printf

## Description

_printf is a custom implementation of the C standard library’s printf function. It produces formatted output to the standard output stream (stdout). This project replicates the functionality of printf with support for basic conversion specifiers.

# Features

Supports the following format specifiers:

- %c: Prints a single character.
- %s: Prints a string.
- %%: Prints a literal %.
- %d / %i: Prints signed decimal integers.

# Usage

## Compilation

To compile the _printf function:

 ' gcc -Wall -Wextra -Werror -pedantic -std=gnu89 *.c -o printf '

## Exmple

''' #include "main.h"

int main(void)
{
    _printf("Character: %c\n", 'H');
    _printf("String: %s\n", "Hello, world!");
    _printf("Integer: %d\n", 12345);
    _printf("Percent sign: %%\n");

    return (0);
}'''

'''Character: H
String: Hello, world!
Integer: 12345
Percent sign: %'''



# Limitations

- Does not handle flag characters (eg. ,+,#, ).
-  Does not support field width or precision.
- Does not handle length modifiers (e.g., l, h).

# Requirements

- Allowed editord 'vi', 'vim', 'emacs'.
- All code must be compiled on Ubuntu 20.04 LTS using gcc with the following options:

''' gcc -Wall -Wextra -Werror -pedantic -std=gnu89 '''

- Code adheres to the Betty coding style.

# Testing 

You can test _printf against the standard printf to verify its output:

'''gcc -Wall -Wextra -Werror -pedantic -std=gnu89 _printf.c main.c _putchar.c -o printf_test
./printf_test'''


# Contrubuting

Contributions, issues, and feature requests are welcome! Feel free to submit a pull request or open an issue on GitHub.

# Author

- [Yavier Maldonado](https://github.com/yavij327)

