# JavaScript Bug: Unexpected String Concatenation
This repository demonstrates a common JavaScript bug related to the `+` operator's behavior with strings.  JavaScript's loose typing system means the `+` operator will concatenate strings rather than performing numeric addition if either operand is a string.

## Bug Description
The provided `foo` function intends to add two numbers. However, if either input is a string, the `+` operator concatenates the values as strings. This results in unexpected outputs.

## How to Reproduce
1. Clone this repository.
2. Run `bug.js` using a JavaScript interpreter (e.g., Node.js).

## Solution
The solution file (`bugSolution.js`) addresses this by explicitly converting the input to numbers using `parseInt()` before the addition to ensure the correct numeric operation.