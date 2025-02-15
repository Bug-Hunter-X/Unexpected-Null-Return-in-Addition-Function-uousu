# Unexpected Null Return in Addition Function

This repository demonstrates a common JavaScript bug involving null handling in a simple addition function. The `foo` function returns null if either input is null, even if the other input is a valid number. This behavior might be unexpected, especially when dealing with potentially null or undefined values from external sources.

The solution focuses on improving the robustness of the function by handling null values more gracefully, either by returning 0 if a null value is provided, or by throwing an error if a null or undefined value is not expected.

## How to Reproduce

1. Clone this repository.
2. Run `bug.js`.
3. Observe the console output. The output will be 3, null, null, null, showcasing the unexpected null return values.
4. Run `bugSolution.js` to observe the solution's improved behavior.

## Solution

The solution addresses the null handling issue by checking for and appropriately handling null or undefined inputs, providing better error handling and predictability.