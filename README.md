# Go Array Index Out of Bounds
This example demonstrates a common error in Go: an array index out of bounds.  The program attempts to access an array element beyond its defined size, resulting in a runtime panic.

## Bug
The `bug.go` file contains a `for` loop that iterates from 0 to 5 (inclusive) when attempting to assign values to an array of size 5. Because array indices are 0-based, the last iteration tries to access `a[5]`, which is out of bounds.  This leads to a runtime panic.

## Solution
The `bugSolution.go` file corrects the bug by changing the loop condition to `i < 5`, ensuring that the loop only iterates up to the valid index range of the array.