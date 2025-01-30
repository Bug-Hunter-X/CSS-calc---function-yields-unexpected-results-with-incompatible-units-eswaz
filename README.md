# CSS `calc()` Compatibility Issue

This repository demonstrates a common issue encountered when using the CSS `calc()` function: incompatible units.  The `calc()` function is powerful, but it requires careful attention to unit compatibility to avoid unexpected layout discrepancies across different browsers and screen sizes.

The `bug.css` file contains the problematic CSS, while `bugSolution.css` offers a corrected and more robust approach.  Read the comments within the code for a more detailed explanation of the problem and its solution.

## Reproducing the Bug

1. Open `bug.html` in your web browser.
2. Observe the layout; the intended behavior might not be achieved consistently across various browsers.

## Understanding the Problem

The core issue stems from using incompatible units within a single `calc()` expression.  Mixing units such as `px` (pixels) and `%` (percentages) can result in unpredictable outcomes because the browsers might evaluate them differently, causing visual differences.

## Solution

The solution involves ensuring unit consistency within the `calc()` function.  This usually means converting all units into a common unit (like pixels) before performing calculations.