# JavaScript NaN Comparison Issue

This repository demonstrates a common pitfall in JavaScript related to comparing NaN (Not a Number) values using loose equality (==).

## The Problem

In JavaScript, NaN is a special value representing an undefined or unrepresentable numerical result.  The loose equality operator (==) does not consider NaN to be equal to itself.  This leads to unexpected results, as shown in the provided code example. 

## Solution

The recommended way to check if a value is NaN is to use the `isNaN()` function. This function correctly identifies NaN, providing the expected behavior.

## How to reproduce

1. Clone this repo.
2. Open bug.js in your preferred code editor.
3. Run the code. Observe that the output is 'false'.
4. Then open the bugSolution.js and run the code. Observe that the output is 'true'.
