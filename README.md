# Unexpected Behavior with Negative Input in TypeScript Function

This repository demonstrates an uncommon bug in a TypeScript function that handles numerical input.  The function `printNumbers` is intended to print numbers from 1 to n. However, when a negative number is passed as input, it unexpectedly does nothing instead of throwing an error or handling the case appropriately.

## Bug Description
The `printNumbers` function fails to handle negative input correctly. It does not print any numbers when a negative integer is supplied as an argument.  Expected behavior would be either no output (silent handling), an error message or printing numbers from 1 to n if the intention is to handle negative numbers as zero. 

## How to Reproduce
1. Clone this repository.
2. Compile the `bug.ts` file using TypeScript compiler (tsc bug.ts).
3. Run the compiled JavaScript file. Observe the unexpected behavior when calling `printNumbers` with a negative argument.

## Solution
The solution involves adding input validation to the function to handle negative numbers appropriately. A revised version is provided in `bugSolution.ts`