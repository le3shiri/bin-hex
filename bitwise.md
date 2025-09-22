Bitwise operations work on the individual bits of numbers, which are usually represented in binary (0s and 1s). Here’s a quick rundown of the key players:
🔧 Bitwise Operators

AND (&): Lights up a bit (1) only if both inputs have that bit on.

Example: 1100 & 1010 = 1000 (only the 4th bit is 1 in both).


OR (|): Lights up a bit (1) if at least one input has that bit on.

Example: 1100 | 1010 = 1110 (combines all 1s).


XOR (^): Lights up a bit (1) only if the inputs are different.

Example: 1100 ^ 1010 = 0110 (1 where bits differ).


NOT (~): Flips every bit (0 becomes 1, 1 becomes 0).

Example (8-bit): ~00001111 = 11110000.



↔️ Bit Shifting
Shifting moves bits left or right, like sliding numbers on a number line:

Left Shift (<<): Moves bits left, multiplying the number by 2 for each shift.

Example: 00011010 (26) << 2 = 01101000 (104) (multiplied by 4).


Right Shift (>>): Moves bits right, dividing the number by 2 for each shift.

Logical Shift: Fills empty spots with 0s.

Example: 00011010 (26) >> 2 = 00000110 (6).


Arithmetic Shift: Copies the sign bit (for negative numbers).

Example: 11100000 (-32) >> 2 = 11111000 (-8).





🎨 Bit Masks
Masks are like stencils that help you focus on specific bits:

Test a bit (check if it’s 1): x & (1 << k) (k is the bit position).
Set a bit (turn it ON): x |= (1 << k).
Clear a bit (turn it OFF): x &= ~(1 << k).
Toggle a bit (flip it): x ^= (1 << k).
Extract a field (get bits from position s to e): (x >> s) & ((1 << (e-s+1)) - 1).