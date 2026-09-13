# C Basics

## 1. Data Types

| Data Type | Description |
| `int` | Used to store whole numbers (positive, negative, or zero) without any decimal point. Typically occupies 4 bytes. |
| `float` | Used to store single-precision floating-point (decimal) numbers. Typically occupies 4 bytes and offers about 6-7 decimal digits of precision. |
| `double` | Used to store double-precision floating-point numbers. Typically occupies 8 bytes and offers greater precision (about 15-16 digits) than `float`. |
| `char` | Used to store a single character (letter, digit, or symbol). Typically occupies 1 byte and internally stores the character's ASCII value. |
| `bool` | Used to store logical values: `true` or `false`. Requires `#include <stdbool.h>` in C, and typically occupies 1 byte. |
| `void` | Represents the absence of a type. Commonly used for functions that do not return a value, or for generic pointers (`void*`). |

## 2. Format Specifiers

| Specifier | Description |
| `%d` | Prints a signed decimal integer. |
| `%u` | Prints an unsigned decimal integer. |
| `%o` | Prints an integer in octal (base 8) format. |
| `%x` | Prints an integer in hexadecimal (base 16) format, using lowercase letters (a-f). |
| `%X` | Prints an integer in hexadecimal (base 16) format, using uppercase letters (A-F). |
| `%f` | Prints a floating-point number in decimal notation. |
| `%e` | Prints a floating-point number in scientific (exponential) notation. |
| `%c` | Prints a single character. |
| `%s` | Prints a string (sequence of characters). |
| `%ld` | Prints a signed `long int` value. |

## 3. Input/Output Functions

**`scanf()`**
Reads formatted input from the user (keyboard) and stores it into variables using format specifiers. Requires the `&` address-of operator for most variable types (except strings/char arrays).
```c
int age;
scanf("%d", &age);
```

**`printf()`**
Prints formatted output to the screen, using format specifiers to control how data types are displayed.
```c
printf("Age: %d\n", age);
```

**`getchar()`**
Reads a single character from the input (keyboard) and returns it. Does not require any format specifier.
```c
char ch = getchar();
```

**`putchar()`**
Prints a single character to the screen.
```c
putchar(ch);
```

**`fgets()`**
Reads a line of text (including spaces) from the input and stores it as a string, up to a specified number of characters. Safer than `gets()` because it prevents buffer overflow.
```c
char name[50];
fgets(name, sizeof(name), stdin);
```

**`puts()`**
Prints a string to the screen and automatically adds a newline at the end.
```c
puts("Hello, World!");
```

## 4. Escape Sequences

| Escape Sequence | Meaning |
| `\n` | Newline — moves the cursor to the next line | `printf("Hello\nWorld");` |
| `\t` | Horizontal tab — inserts a tab space | `printf("Name:\tAli");` |
| `\\` | Backslash — prints a literal backslash character | `printf("C:\\Users");` |
| `\'` | Single quote — prints a literal single quote | `printf("It\'s C");` |
| `\"` | Double quote — prints a literal double quote inside a string | `printf("She said \"Hi\"");` |
| `\0` | Null character — marks the end of a string | Used internally to terminate strings |

## 5. Precision

Precision for floating-point output is specified in `printf()` by placing a **period followed by a number** between the `%` sign and the conversion character (e.g., `f`). This number tells the compiler how many digits to display after the decimal point.

```c
float pi = 3.14159265;

printf("%.2f\n", pi);   // Output: 3.14
printf("%.4f\n", pi);   // Output: 3.1416
printf("%.0f\n", pi);   // Output: 3
```

- `%.2f` rounds and displays 2 digits after the decimal point.
- `%.4f` rounds and displays 4 digits after the decimal point.
- If no precision is specified, `printf()` defaults to 6 digits after the decimal point.

Precision can also be combined with field width, e.g., `%10.2f` reserves a total width of 10 characters while showing 2 decimal digits.
