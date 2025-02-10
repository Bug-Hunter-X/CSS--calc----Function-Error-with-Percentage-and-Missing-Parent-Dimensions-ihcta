# CSS `calc()` Function Error with Percentage and Missing Parent Dimensions

This repository demonstrates a subtle bug related to the CSS `calc()` function and the handling of percentage values when the parent element lacks explicitly defined dimensions.

## The Problem

The `calc()` function is powerful, but it can produce unexpected results if not used carefully.  The issue arises when you use percentages within `calc()` and the parent element doesn't have its width and height set explicitly.

## Reproducing the Bug

1. Clone this repository.
2. Open `index.html` in your web browser.
3. Observe that the element's width and height are incorrect, despite the use of `calc()`.

## Solution

The solution involves adding explicit width and height values to the parent container element so that `calc()` can correctly resolve the percentage values. This is demonstrated in `bugSolution.css`.

## Lessons Learned

- Always ensure parent elements have defined dimensions when using percentages within the CSS `calc()` function to avoid unexpected results.
- Carefully test your CSS code under various scenarios to catch these subtle errors.
