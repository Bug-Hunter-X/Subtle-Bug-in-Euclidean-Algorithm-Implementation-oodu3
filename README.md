# Subtle Bug in Euclidean Algorithm Implementation

This repository demonstrates a subtle bug in a JavaScript implementation of the Euclidean algorithm for finding the greatest common divisor (GCD) of two numbers.  The bug manifests when one number is a multiple of the other.

## Bug Description
The provided `foo` function attempts to recursively calculate the GCD. While it generally works, it fails when `a` is a multiple of `b` (or vice-versa) and returns an incorrect result. This is due to a condition error in the algorithm's handling of the base case.

## Bug Reproduction
The `bug.js` file contains the buggy implementation. Run it to observe the incorrect outputs.

## Solution
The `bugSolution.js` file provides a corrected implementation that addresses the bug. The key change lies in how the base case for the recursion is handled.