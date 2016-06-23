### brainstack
A simple program used to implement a stack in Brainfuck.

## How to use:

Use your favorite Brainfuck compiler/interpreter on `source/tictactoe` to play the game. [Recommendation](https://github.com/iarba/bfcompiler)

## Program

The program represents a simple conversation protocol with the computer. The computer memorises all values that are not 10(`'\n'`) or 33(`'!'`), and pushes the value in a stack.

When the value 10(`'\n'`) is inserted, the computer pops the value at the top of the stack and prints it out.

Value 33(`'!'`) terminates the execution.

## Implementation

The stack is placed at position 64 and uses 2 bytes per value inserted. The head of the stack(64 and 65) are always empty, to represent the start of the stack. The stack can be accessed from anywhere in the program where you know the absolute distance between the current pointer and the stack pointer.

If the stack grows too big, it may run over other memory locations or overflow the memory, so don't abuse it.

