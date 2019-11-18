# Rotary

Rotary is a programming language inspired by the rotary phone dial. Each command is placed into a several-deep rotary wheel. On each line of the program, the wheel is placed back at the initial spot. The `>` character moves the wheel to the right, `^` is used to move up a layer, and `.` is used to move the wheel back to its beginning location. Each value is read and stored as an integer, and characters are printed according to their unicode value.

The wheel is layed out in four layers:

4. Registers: 8 registers to store values
3. Flow: Create label, jump to label, jump if zero, jump of negative, exit
2. Arithmetic: + - * / %
1. I/O: Read integer, read character, print integer, print character
