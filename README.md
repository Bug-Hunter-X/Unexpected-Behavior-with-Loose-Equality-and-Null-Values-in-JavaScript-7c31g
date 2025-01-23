# Unexpected Behavior with Loose Equality and Null Values in JavaScript

This code demonstrates a common error in JavaScript involving loose equality (`==`) and comparisons with `null` or `undefined`.  Loose equality can lead to unexpected behavior, particularly when comparing values of different types or involving `null`.

## The Problem

The `foo` function uses loose equality (`===`) to check for `null` values. While it works for the explicit `null` checks, it can be problematic if other falsy values (e.g., 0, false, "") are involved.  This can lead to incorrect results or unexpected behavior in your application.

## The Solution

The solution provided uses strict equality (`===`) for more precise comparisons. Strict equality checks both value and type, preventing the unexpected behavior caused by loose equality.

## How to Reproduce the Bug

1. Clone this repository.
2. Run `node bug.js` in your terminal. Observe the output which shows the unexpected behaviour. 
3. Run `node bugSolution.js`. Observe the output which shows the corrected behaviour. 
