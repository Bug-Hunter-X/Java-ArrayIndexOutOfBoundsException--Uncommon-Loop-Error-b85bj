# Java ArrayIndexOutOfBoundsException: An Uncommon Loop Error
This repository demonstrates a subtle ArrayIndexOutOfBoundsException in Java, highlighting an easily overlooked error in array traversal.
The bug stems from an off-by-one error in a `for` loop's termination condition.  The loop attempts to access an index beyond the array's bounds, leading to the exception. This example illustrates the importance of careful loop index management when working with arrays in Java.
## How to Reproduce
1. Clone this repository.
2. Compile and run the `bug.java` file.  You'll observe an `ArrayIndexOutOfBoundsException`.
3. Examine the `bugSolution.java` file for the corrected code.
## Solution
The solution involves simply changing the loop condition from `i <= arr.length` to `i < arr.length`. This ensures that the loop iterates only within the valid index range of the array.