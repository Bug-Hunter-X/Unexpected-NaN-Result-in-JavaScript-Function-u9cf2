# Unexpected NaN Result in JavaScript Function

This repository demonstrates a common JavaScript error: unexpected NaN results when null values are passed to a function that performs arithmetic operations without proper null handling.

The `bug.js` file contains the faulty code, which does not check for null values before performing calculations. This leads to NaN (Not a Number) being returned.

The `bugSolution.js` file provides a corrected version of the code. It adds null checks to prevent NaN errors and provides more robust handling of potential null or undefined values.

## Bug Report

The bug occurs in the `bar` function.  When a null value is passed as an argument to the `foo` function, it causes a NaN to be generated, and this propagates to the result of `bar` function.

## Solution

The solution involves adding explicit checks for null or undefined values before performing arithmetic operations.