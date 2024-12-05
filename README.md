# Off-by-One Error in C++ Vector Iteration

This repository demonstrates a common off-by-one error in C++ when iterating over a `std::vector`.  The error occurs because the loop condition `i <= vec.size()` attempts to access an element beyond the valid range of the vector.

## Bug
The `bug.cpp` file contains the erroneous code.  The for loop's condition should be `i < vec.size()` to avoid accessing an element outside of the vector's bounds. 

## Solution
The `bugSolution.cpp` file provides a corrected version of the code.

## How to reproduce
1. Clone this repository.
2. Compile and run `bug.cpp` (expect undefined behavior or a crash).
3. Compile and run `bugSolution.cpp` (expect correct output).