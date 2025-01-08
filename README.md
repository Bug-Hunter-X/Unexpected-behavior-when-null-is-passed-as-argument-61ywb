# Unexpected Null Handling in JavaScript Function

This repository demonstrates a common JavaScript bug involving unexpected behavior when `null` values are passed as arguments to a function.  The function `foo` silently returns without explicitly handling `null` values, potentially leading to unexpected program behavior or silent failures.

## Bug Description
The `foo` function does not explicitly check for or handle `null` values passed as arguments. This results in the function silently exiting without any error or warning, potentially masking a problem and making debugging more challenging.

## Solution
The provided solution explicitly checks for `null` values using strict equality (`===`) and either throws an error, returns a default value, or performs alternate logic as appropriate.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js` and `bugSolution.js`.
3. Run `bug.js` and observe the function's unexpected behavior with null arguments.
4. Compare this to the behavior in `bugSolution.js`. 