# CSS :nth-child Specificity Issue in Nested Lists

This repository demonstrates an uncommon issue related to CSS selector specificity when using the `:nth-child` pseudo-class in nested lists. The problem arises from the cumulative counting of elements within nested structures, leading to unexpected styling.

## Problem Description

The provided CSS attempts to alternate background colors for list items. However, when nested lists are present, the counting is not confined to each individual list, resulting in incorrect styling application.  See the `bug.css` file for the problematic code.

## Solution

The solution involves using the `:nth-child` pseudo-class with a scope to address the issue.  This scoping ensures that counting happens within the immediate parent list.  See `bugSolution.css` for the corrected code.

## How to Reproduce

1. Clone this repository.
2. Open `index.html` in a web browser (you'll need to create a simple `index.html` with the nested lists). 
3. Observe the incorrect and then corrected styling.