# Problem Set Two
### CS 3053 Operating Systems

## Problem One - Stack Machine based on Linked List

Using the **prob1.c** starter file, implement a stack machine using a linked list to store operands(strings).  The stack will be populated with operands from standard input (stdin). Each line from stdin will consist of a command and an operand.  The format will be *command:operand*.  Each of the commands will correspond to a function implemented in your program. Your program will need to implement the following *commands/functions* that are specified in your starter file:

* push - Add a new node to the top of the stack
* pop  - Remove the top node from the stack
* show - Display the nodes on the stack

You must implement each of these functions in your starter file.  You may create any additional functions you need.  The only two C standard libraries available to you are *<stdio.h>* and *<stdlib.h>*. No global variables. (A struct definition is not a variable)

### Example Input
```
push:Apples
push:Oranges
show:
pop:
push:Bananas
show:
```
### Output
```
[0xbf094330]
Operand: Oranges
Next: [0xbf094300]

[0xbf094300]
Operand: Apples
Next: [0x0]

[0xbf094400]
Operand: Bananas
Next: [0xbf094300]

[0xbf094300]
Operand: Apples
Next: [0x0]
```


