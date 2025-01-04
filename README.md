# Assembly Integer Overflow in Memory Access

This repository demonstrates a potential integer overflow bug in assembly code that can lead to incorrect memory access.

The `bug.asm` file contains the erroneous code, while `bugSolution.asm` provides a corrected version that handles potential overflows.

## Bug Description
The bug stems from a lack of bounds checking on the ECX register before using it in an address calculation. If ECX is too large, the multiplication will cause an overflow.

## Solution
The solution involves adding code to check the value of ECX before performing the calculation and handling overflow appropriately. The improved code in `bugSolution.asm` demonstrates this fix.