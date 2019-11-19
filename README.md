# Rotary

Rotary is a programming language inspired by the rotary phone dial. Each command is placed into a several-deep rotary wheel. On each line of the program, the wheel is placed back at the initial spot. The `>` character moves the wheel to the right, `^` is used to move up a layer, a `.` is used to move the current wheel back to the left while traversing a row, or to move the wheel to its starting position wheel layer if currently in the first location of a row. Each value is read and stored as an integer, and characters are printed according to their unicode value.

The wheel is layed out in four layers:

1. Storage: Data stores for values or line labels, can be pushed to like a stack
2. Flow: Create label, jump to label, jump if zero, jump of negative, exit
3. Arithmetic: + - * / %
4. I/O: Read integer, read character, print integer, print character

Translated into a rotary dial, it might look like so:

## Example

A simple program that takes two numbers, adds them, and displays the result, would look like so:

```
>.^^^      # Read an integer and push to stack
>.^^^
^>.^^>.>>. # Add the first and second values and push it to the registers
>>.^^^>    # Print first value from registers
```
