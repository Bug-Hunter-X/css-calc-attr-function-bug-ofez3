# CSS calc() and attr() Bug

This repository demonstrates a common error when using the `calc()` function with the `attr()` function in CSS.  Specifically, it highlights the issue of missing or incorrect units when fetching values from the `data-offset` attribute.

The `bug.css` file contains the problematic code. The `bugSolution.css` file provides the corrected version.

## Problem
The issue arises when the `data-offset` attribute does not contain a valid unit (like `px`, `em`, `%`, etc.).  The `calc()` function expects numerical values with units, and attempting to perform calculations without them will often lead to incorrect rendering or unexpected behavior.

## Solution
The solution involves adding a unit to the `attr()` function and providing fallback values to gracefully handle scenarios where the attribute is missing or contains an invalid value.

## Usage
1. Clone the repository.
2. Open the `bug.html` (or a similar test file) to see the rendering issue.
3. Replace the CSS with the corrected version to fix the issue.