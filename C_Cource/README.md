# C language


## Why Learn C?
Efficiency: C is a low-level language, which allows you to work directly with memory and hardware.
Portability: Programs written in C can be compiled and run on many different platforms with little or no modification.
Foundation for Other Languages: Many modern programming languages like C++, Java, and Python have their roots in C.
Wide Usage: C is widely used in system programming, embedded systems, operating systems, and more.

## Structure of a C Program
```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

## Steps to Run a C Program:
1. Write the code in a **.c** file (e.g., **hello.c**).
2. Compile the code using a C compiler (e.g., gcc for Linux/Windows/macOS). Example:
    ```bash
    gcc hello.c -o hello
    ```
3. Run the executable:
    ```bash
    ./hello   (on Linux/macOS)
    hello.exe (on Windows)
    ```

## Basic Syntax:
- Variables: Used to store data.
    ```c
    int a = 10;
    float b = 5.25;
    char c = 'A';
    ```

- Data Types:

    - int: Integer (e.g., 1, 2, -3).
    - float: Floating-point number (e.g., 1.23, 4.56).
    - char: Single character (e.g., 'a', 'b').
- Operators:

    - Arithmetic: +, -, *, /, % (modulus).
    - Comparison: ==, !=, >, <, >=, <=.
    - Logical: &&, ||, !.

Example Program: Basic Arithmetic
```c
#include <stdio.h>

int main() {
    int a = 10, b = 20;
    int sum = a + b;
    printf("Sum: %d\n", sum);
    return 0;
}
```
## Operators

- ### Arithmetic Operators:

    | Operator   | Operation      | Example       |
    |------------|----------------|---------------|
    | `+`        | Addition       | `a + b`       |
    | `-`        | Subtraction    | `a - b`       |
    | `*`        | Multiplication | `a * b`       |
    | `/`        | Division       | `a / b`       |
    | `%`        | Modulus        | `a % b`       |

- ### Comparison Operators:
    | Operator   | Operation                  | Example       |
    |------------|----------------------------|---------------|
    | `+`        | Addition                   | `a + b`       |
    | `-`        | Subtraction                | `a - b`       |
    | `*`        | Multiplication             | `a * b`       |
    | `/`        | Division                   | `a / b`       |
    | `%`        | Modulus                    | `a % b`       |
    | `==`       | Equal to                   | `a == b`      |
    | `!=`       | Not equal to               | `a != b`      |
    | `>`        | Greater than               | `a > b`       |
    | `<`        | Less than                  | `a < b`       |
    | `>=`       | Greater than or equal to   | `a >= b`      |
    | `<=`       | Less than or equal to      | `a <= b`      |


- ### Logical Operators:
    | Operator   | Operation                  | Example       |
    |------------|----------------------------|---------------|
    | `&&`       | Logical AND                | `a && b`      |
    | `||`       | Logical OR                 | `a || b`      |
    | `!`        | Logical NOT                | `!a`          |
    | `&`        | Bitwise AND                | `a & b`       |
    | `|`        | Bitwise OR                 | `a | b`       |
    | `^`        | Bitwise XOR                | `a ^ b`       |
    | `~`        | Bitwise NOT                | `~a`          |
    | `<<`       | Left shift                 | `a << b`      |
    | `>>`       | Right shift                | `a >> b`      |



## Control Structures

- ### If-Else Statements
- ### Switch Statements
- ### Loops 
    - #### For Loop
    - #### While Loop
    - #### Do-While Loop: The body of the loop executes at least once.


| Control Structure | Description                                        | Example                                                   |
|-------------------|----------------------------------------------------|-----------------------------------------------------------|
| `if`              | Executes a block of code if the condition is true  | `if (condition) { /* code */ }`                           |
| `else`            | Executes a block of code if the condition is false | `if (condition) { /* code */ } else { /* code */ }`       |
| `else if`         | Checks another condition if the previous is false  | `if (condition) { /* code */ } else if (condition) { /* code */ } else { /* code */ }` |
| `switch`          | Selects one of many blocks of code to execute      | `switch (expression) { case value: /* code */ break; }`    |
| `for`             | Loops a block of code a specified number of times  | `for (init; condition; increment) { /* code */ }`          |
| `while`           | Loops a block of code while the condition is true  | `while (condition) { /* code */ }`                        |
| `do...while`      | Executes a block of code, then checks condition    | `do { /* code */ } while (condition);`                    |
| `break`           | Exits a loop or `switch` statement                | `break;`                                                  |
| `continue`        | Skips the rest of the current iteration of a loop  | `continue;`                                               |
| `goto`            | Jumps to a labeled statement                       | `goto label; ... label: /* code */`                       |
| `return`          | Exits from a function and optionally returns a value | `return value;`                                           |



## Functions
Functions allow you to reuse code and make your programs modular.

**Function Syntax**:
```c
return_type function_name(parameter1, parameter2, ...) {
    // Function body
    return value; // if the function returns a value
}
```

**Example: Simple Function**
```c
#include <stdio.h>

// Function declaration
int add(int a, int b);

int main() {
    int result = add(5, 3);
    printf("Sum: %d\n", result);
    return 0;
}

// Function definition
int add(int a, int b) {
    return a + b;
}
```

## Arrays
An array is a collection of variables of the same type, stored in contiguous memory locations. Arrays allow you to store multiple values in a single variable, which can be accessed using an index.

**Declaring an Array:**
```c
data_type array_name[array_size];
```

#### Example: Declaring and Initializing an Array
```c
int numbers[5] = {10, 20, 30, 40, 50};
```
#### Accessing Array Elements:
```c
int first_element = numbers[0];  // Accesses the first element (10)
numbers[2] = 35;  // Changes the third element to 35
```

**Example Program: Working with Arrays**
```c
#include <stdio.h>

int main() {
    int numbers[5] = {1, 2, 3, 4, 5};

    // Printing the array elements
    for (int i = 0; i < 5; i++) {
        printf("Element at index %d: %d\n", i, numbers[i]);
    }

    return 0;
}
```

## Pointers
A pointer is a variable that stores the memory address of another variable. Pointers are powerful because they allow direct access and manipulation of memory, enabling efficient programming.


**Declaring a Pointer:**
```c
data_type *pointer_name;
```

**Example: Declaring and Using a Pointer**
```c
int num = 10;
int *ptr = &num;  // Pointer to the address of 'num'

printf("Value of num: %d\n", num);         // Outputs 10
printf("Address of num: %p\n", &num);      // Outputs the memory address of num
printf("Value stored in ptr: %p\n", ptr);  // Outputs the address of num (same as above)
printf("Value pointed by ptr: %d\n", *ptr);// Outputs 10 (value at the memory address)
```

**Example: Pointer Arithmetic**
```c
#include <stdio.h>

int main() {
    int numbers[3] = {10, 20, 30};
    int *ptr = numbers;  // Pointing to the first element of the array

    printf("First element: %d\n", *ptr);    // 10
    ptr++;                                  // Move to the next element
    printf("Second element: %d\n", *ptr);   // 20
    ptr++;
    printf("Third element: %d\n", *ptr);    // 30

    return 0;
}
```
### Pointers and Arrays
In C, arrays and pointers are closely related. When you pass an array to a function, what actually gets passed is a pointer to the first element of the array.

**Example: Passing an Array to a Function**
```c
#include <stdio.h>

void printArray(int *arr, int size) {
    for (int i = 0; i < size; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
}

int main() {
    int numbers[5] = {1, 2, 3, 4, 5};
    printArray(numbers, 5);  // Passing the array
    return 0;
}
```

## Pointer to Pointer
A pointer to pointer is a pointer that stores the address of another pointer. It’s useful in scenarios where you want to manipulate pointers or work with dynamic memory allocation.

**Example: Pointer to Pointer**
```c
#include <stdio.h>

int main() {
    int num = 10;
    int *ptr = &num;     // Pointer to num
    int **ptr2 = &ptr;   // Pointer to ptr

    printf("Value of num: %d\n", num);        // 10
    printf("Value of num via ptr: %d\n", *ptr); // 10
    printf("Value of num via ptr2: %d\n", **ptr2); // 10

    return 0;
}
```

### Size of Pointers
The size of a pointer in C depends on the system's architecture (whether it’s 32-bit or 64-bit). Typically, on:

- `32-bit systems`: A pointer is usually `4 bytes` (32 bits).
- `64-bit systems`: A pointer is usually `8 bytes` (64 bits).
However, the size of the pointer is ``independent`` of the type of data it points to. Whether it points to an int, char, float, or a structure, `the pointer itself will have the same size. What changes is the amount of memory the pointer is referencing.`

```c
#include <stdio.h>

int main() {
    int *intPtr;
    char *charPtr;
    double *doublePtr;

    printf("Size of int pointer: %lu bytes\n", sizeof(intPtr)); // Size of int pointer: 8 bytes
    printf("Size of char pointer: %lu bytes\n", sizeof(charPtr)); // Size of char pointer: 8 bytes
    printf("Size of double pointer: %lu bytes\n", sizeof(doublePtr)); // Size of double pointer: 8 bytes

    return 0;
}
```

## Types of Pointers
- #### Null Pointer
- #### Void Pointer (Generic Pointer)
- #### Dangling Pointer
- #### Wild Pointer
- #### Function Pointer
- #### Pointer to Pointer (Double Pointer)

### Null Pointer

A null pointer is a pointer that doesn't point to any valid memory location. It is often used to indicate that the pointer is not currently pointing at an object.

- A null pointer is created by assigning `NULL` or `0` to the pointer.
- It's a good practice to initialize unused pointers as `NULL` to avoid accidental use of uninitialized pointers.

```c
#include <stdio.h>

int main() {
    int *ptr = NULL;  // or ptr = 0;
    
    if (ptr == NULL) {
        printf("Pointer is null\n");
    }

    return 0;
}
```

### Void Pointer (Generic Pointer)

A **void pointer** is a pointer that can point to any data type. However, it cannot be dereferenced directly, and must be `cast` to another pointer type before dereferencing.

```c
#include <stdio.h>

int main() {
    int num = 10;
    void *ptr = &num;  // Void pointer

    // Dereferencing the void pointer requires type casting
    printf("Value of num: %d\n", *(int *)ptr);  // Casting to int pointer

    return 0;
}
```
### Dangling Pointer
A `dangling pointer` points to a memory location that has been freed or deallocated. Dereferencing a dangling pointer can lead to undefined behavior, as it no longer points to valid memory.

To avoid dangling pointers, always set a pointer to `NULL` after freeing the memory it points to.

```c
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *ptr = (int *)malloc(sizeof(int));  // Dynamic memory allocation
    *ptr = 42;

    free(ptr);  // De-allocating the memory
    ptr = NULL; // Preventing a dangling pointer

    return 0;
}
```


### Wild Pointer

A **wild pointer** is an uninitialized pointer, meaning it points to some arbitrary memory location. Accessing or dereferencing such a pointer will result in unpredictable behavior.

To avoid wild pointers, always initialize pointers (e.g., to `NULL` or a valid memory address).
```c
int *wildPtr;  // This is a wild pointer
wildPtr = NULL;  // Now it's initialized to NULL
```

### Function Pointer
A **function pointer** points to the address of a function. This allows functions to be passed as arguments to other functions, enabling dynamic execution of functions.

```c
#include <stdio.h>

// Function declaration
void printMessage() {
    printf("Hello, World!\n");
}

int main() {
    void (*funcPtr)() = printMessage;  // Function pointer

    // Calling the function via the pointer
    (*funcPtr)();  // or just funcPtr();

    return 0;
}
```

### Pointer to Pointer (Double Pointer)

A `pointer to pointer` (or double pointer) stores the address of another pointer. It is particularly useful when dealing with dynamic memory, arrays of pointers, or functions that modify pointers.

```c
#include <stdio.h>

int main() {
    int num = 10;
    int *ptr = &num;     // Pointer to num
    int **ptr2 = &ptr;   // Pointer to ptr (double pointer)

    printf("Value of num: %d\n", **ptr2);  // Dereferencing twice to get the value

    return 0;
}
```







