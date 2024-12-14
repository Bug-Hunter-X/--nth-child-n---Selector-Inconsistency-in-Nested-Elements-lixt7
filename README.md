# :nth-child(n) Selector Issue in Nested CSS

This repository demonstrates an uncommon issue with the CSS `:nth-child(n)` selector when applied to nested elements.  The selector sometimes behaves inconsistently when the parent container's structure or child count changes dynamically.

## Problem Description
The `bug.css` file contains CSS code using `:nth-child(n)` to style specific elements within a nested structure. Under certain conditions (e.g., adding or removing elements, modifying the DOM dynamically), the styling applied by `:nth-child(n)` may not reflect the actual order or position of the elements.

## Solution
The `solution.css` file provides alternative methods to achieve the desired styling, avoiding the inconsistencies of `:nth-child(n)` in complex scenarios.  Solutions may include using JavaScript to manipulate classes or a more robust selector that's less affected by structural changes.

## How to reproduce
1. Clone this repository.
2. Open `index.html` (not included in this repo, you will have to create one) in your browser.
3. Observe the initial styling.
4. Manipulate the elements in the DOM (using browser developer tools, for example). Note how the styling changes (or doesn't change) as expected.
