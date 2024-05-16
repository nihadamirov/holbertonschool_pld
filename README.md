# Monty Language Interpreter

This project is an interpreter for the Monty language, written in C. It uses a doubly linked list to represent a stack (or queue), and supports a variety of operations.

## About the Monty Language

The Monty language is a scripting language that is compiled into Monty bytecodes. It relies on a unique stack, with specific instructions to manipulate it.

## Stack Data Structure

The stack data structure used in this project is represented by the following structure:

```c
typedef struct stack_s
{
    int n;
    struct stack_s *prev;
    struct stack_s *next;
} stack_t;
```

This structure represents a doubly linked list node for stack, queues, LIFO (Last In, First Out), and FIFO (First In, First Out) operations.

## Operations

The following operations are implemented in this project:

- `PUSH`: Adds an element to the stack.
- `PALL`: Prints all the values on the stack, starting from the top of the stack.
- `PINT`: Prints the value at the top of the stack.
- `POP`: Removes the top element of the stack.
- `SWAP`: Swaps the top two elements of the stack.
- `ADD`: Adds the top two elements of the stack.

## How to Use

To use this Monty language interpreter, compile the C files in this repository and run the resulting executable with a `.m` file as an argument. The `.m` file should contain Monty bytecodes.

Here is an example of how to compile and run the program:

```bash
gcc *.c -o monty
./monty bytecode_file.m
```

