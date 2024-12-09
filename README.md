# Division by Zero Bug in C++

This repository demonstrates a common error in C++: division by zero. The code attempts to divide an integer by zero, which leads to undefined behavior.

## Bug Description

The `bug.cpp` file contains a simple C++ program that initializes two integer variables, `x` and `y`, and then attempts to divide `x` by `y`, where `y` is 0. This results in a division by zero error.  The program may crash, produce incorrect results, or behave erratically.

## Solution

The `bugSolution.cpp` file provides a corrected version of the code. It includes a check to prevent division by zero before attempting the division. This ensures that the program handles the case of a zero divisor gracefully. 

## How to reproduce the bug

1. Compile `bug.cpp` using a C++ compiler (like g++):
   ```bash
   g++ bug.cpp -o bug
   ```
2. Run the compiled executable:
   ```bash
   ./bug
   ```
You should observe undefined behavior, possibly a segmentation fault.

## How to test the solution

1. Compile `bugSolution.cpp`:
   ```bash
   g++ bugSolution.cpp -o bugSolution
   ```
2. Run the compiled executable:
   ```bash
   ./bugSolution
   ```
The output should indicate that division by zero was prevented.
