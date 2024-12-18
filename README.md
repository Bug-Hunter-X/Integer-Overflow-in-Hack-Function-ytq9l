# Integer Overflow Bug in Hack

This repository demonstrates a subtle integer overflow bug in a simple Hack program. The function `baz` calculates `(x + 1) * 2 - 1`, which could overflow if x is sufficiently large. 

## Bug Description

The `baz` function might produce unexpected results due to integer overflow when the intermediate result of the calculation exceeds the maximum value that can be represented by the Hack's int type.  This may lead to incorrect behavior or crashes.  This demonstrates a potential problem in Hack code where the intermediate results during calculations are not explicitly checked for overflow conditions.

## How to Reproduce

1. Compile the Hack code using the Hack compiler.
2. Run the compiled code.
3. Observe the output.  If the input is large enough, you will see that the result is incorrect due to integer overflow.

## Solution

The provided solution adds checks to prevent this overflow.  This example is simple and can be applied to more complex scenarios by adjusting the checks according to the specific context.

