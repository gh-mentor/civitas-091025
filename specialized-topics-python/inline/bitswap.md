## Conditional Bit Swap in Python

Given the following:

    Mask: 0b1010
    Array 1: [0b1010, 0b1100, 0b1111]
    Array 2: [0b0110, 0b0011, 0b0000]

How would you use prompt engineering to generate a transformation procedure in Python that produces the following result for arrays of equal length?

    Array 1: [0b0010, 0b0110, 0b0101]
    Array 2: [0b1110, 0b1001, 0b1010]

Write a Python function `conditional_bit_swap(arr1, arr2, mask)` that swaps the bits in the same positions of the elements of two integer arrays, but only if the corresponding bit in the mask is set and the bits to be swapped are different. The function should modify the arrays in place.

Show robust unit tests for `conditional_bit_swap` using pytest or unittest, covering at least three different cases with different mask values and array sizes. Use assert statements to check that the output of the function is as expected, and print a message indicating that all tests pass if successful.


Implementation details:

- the conditionalBitSwap function swaps the bits in the same positions

   of the elements of two char arrays, but only if the corresponding bit

   in the mask is set and the bits to be swapped are different.

- the conditionalBitSwap function should not return anything.


