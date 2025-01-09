# Inconsistent Height Calculation with Nested calc() in CSS

This repository demonstrates an uncommon issue related to nested `calc()` functions in CSS.  The problem arises from inconsistencies in how different browsers interpret nested calculations, particularly when mixing percentage and pixel values.

The `bug.css` file contains the problematic CSS code. The `bugSolution.css` file shows a solution to avoid nested `calc()`.

## Problem

The primary issue is how the browser parses the nested `calc()` functions.  Inconsistent parsing can result in the height of `.element` being calculated incorrectly across different browsers.

## Solution

To resolve this issue, it's recommended to avoid nested `calc()` functions whenever possible.  Instead, calculate the values separately and use the results in the CSS.  This ensures consistent calculation and avoids potential browser-specific rendering issues.