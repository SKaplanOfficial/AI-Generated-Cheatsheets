# Booth's Algorithm Cheatsheet

## Overview
- Booth's algorithm is a multiplication algorithm that allows signed binary numbers to be multiplied.
- is named after Andrew Donald Booth, who developed it in 1950.

## Algorithm Steps
1. Align the multiplicand and multiplier, and add a sign bit to the product register.
2. Initialize the multiplier and the product register.
3. Repeat the following steps until the multiplier becomes zero:
   - If the last two bits of the multiplier are 01, add the multiplicand to the product register.
   - If the last two bits of the multiplier are 10, subtract the multiplicand from the product register.
   - Right shift the multiplier and the product register by one bit.

## Example
```
Multiplicand = 0011
Multiplier = 1010

Step 1: Align the numbers
  0011
x 1010
-----
  0011

Step 2: Initialize the algorithm
Multiplier = 1010
Product    = 00000011

Step 3: Repeat until the multiplier becomes zero
Multiplier = 0101
Product    = 00000011

Multiplier = 0010
Product    = 00000011

Multiplier = 0001
Product    = 00000011 - 0011 = 11111100 (2's complement)

Multiplier = 0000
Product    = 11111100 (2's complement) = -4 (in decimal)

Result = -4
```

## Resources
- [Booth's Algorithm Wikipedia](https://en.wikipedia.org/wiki/Booth%27s_multiplication_algorithm)
- [Booth's Algorithm Tutorial](https://www.tutorialspoint.com/booth-algorithm-for-binary-multiplication)