# Implicit Type Coercion in JavaScript

This repository demonstrates a common, yet subtle, error in JavaScript related to implicit type coercion.  The `foo` function attempts to add a number and a string.  Instead of throwing a type error (as one might expect in a strongly-typed language), JavaScript implicitly converts the number to a string and performs string concatenation.

This behavior can lead to unexpected results and hard-to-debug errors in larger applications.  The solution highlights the importance of explicit type checking or using functions designed to handle different data types gracefully.

## How to reproduce

1. Clone this repository.
2. Run `node bug.js` to see the unexpected output.
3. Examine `bugSolution.js` for a corrected version of the function.