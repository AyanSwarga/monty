##### C - Stacks, Queues - LIFO, FIFO

### C Group project Algorithm Data structure

## What is Stack in C?
A stack in C is nothing but a linear data structure that follows the LIFO rule (Last In First Out). In a stack, both insertion and deletion take place from just one end, that is, from the top.

## What is a Queue in C?
In contrast to a stack, a queue in C is nothing but a linear data structure that follows the FIFO rule (First In First Out). Insertion is done from the back (the rear end) and deletion is done from the front.

## Resources
Read or watch:

Google
How do I use extern to share variables between source files in C?
Stacks and Queues in C
Stack operations
Queue operations
## Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:

## General
What do LIFO and FIFO mean
What is a stack, and when to use it
What is a queue, and when to use it
What are the common implementations of stacks and queues
What are the most common use cases of stacks and queues
What is the proper way to use global variables
## Tests
We strongly encourage you to work all together on a set of tests

## The Monty language
Monty 0.98 is a scripting language that is first compiled into Monty byte codes (Just like Python). It relies on a unique stack, with specific instructions to manipulate it. The goal of this project is to create an interpreter for Monty ByteCodes files.

Monty byte code files

Files containing Monty byte codes usually have the .m extension. Most of the industry uses this standard but it is not required by the specification of the language. There is not more than one instruction per line. There can be any number of spaces before or after the opcode and its argument:
Monty byte code files can contain blank lines (empty or made of spaces only, and any additional text after the opcode or its required argument is not taken into account:
## The monty program

-Usage: monty file
-where file is the path to the file containing Monty byte code
-If the user does not give any file or more than one argument to your program, print the error message USAGE: monty file, followed by a new line, and exit with the status EXIT_FAILURE
-If, for any reason, it’s not possible to open the file, print the error message Error: Can't open file <file>, followed by a new line, and exit with the status EXIT_FAILURE
-where <file> is the name of the file
-If the file contains an invalid instruction, print the error message L<line_number>: unknown instruction <opcode>, followed by a new line, and exit with the status EXIT_FAILURE
-where is the line number where the instruction appears.
-Line numbers always start at 1
-The monty program runs the bytecodes line by line and stop if either:
 it executed properly every line of the file
 it finds an error in the file
 an error occured
-If you can’t malloc anymore, print the error message Error: malloc failed, followed by a new line, and exit with status EXIT_FAILURE.
-You have to use malloc and free and are not allowed to use any other function from man malloc (realloc, calloc, …)
