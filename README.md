# Unexpected Behavior in CSS calc() due to Spacing

This repository demonstrates a subtle but important bug in using the `calc()` function in CSS.  Incorrect spacing within the `calc()` expression can lead to unexpected results in certain browsers.

## Bug Description
Spaces around the operators in a `calc()` expression can cause the calculation to fail or produce an incorrect result.  This is not always consistently handled across different browsers.

## How to Reproduce
1. Open `bug.css`.
2. Observe that the width of the `.element` class is not calculated correctly because of the spaces in the `calc()` expression.
3. Open `bugSolution.css`. Note the corrected code without extra spaces in the `calc()` expression.

## Solution
Ensure there are no unnecessary spaces within the parentheses of a `calc()` expression. Keep the operators and operands together to ensure consistent cross-browser compatibility.