# CSS Specificity Gotcha: Unexpected Color Inheritance

This repository demonstrates a subtle CSS specificity issue that can lead to unexpected color inheritance in nested elements.  The problem arises from the interaction between element selectors and nested selectors, and how CSS specificity rules determine which styles are applied.

## Problem Description

The `bug.css` file contains CSS rules that intend to style paragraphs differently based on their context. However, due to specificity, the expected colors are not always applied. 

## Solution

The `bugSolution.css` file provides a corrected version of the CSS, addressing the specificity problem and ensuring the intended styling behavior.

## How to Reproduce

1. Clone this repository.
2. Open `bug.html` (you will need to create a simple HTML file with the structure described in the comments of the CSS file).
3. Observe the colors of the paragraphs; you will see that they don't match the expected colors in the initial CSS.
4. Replace `bug.css` with `bugSolution.css` and refresh the page. The colors will now match the expected values.

## Learning Points

This example highlights the importance of understanding CSS specificity.  Knowing how specificity rules determine which styles are applied is crucial for writing predictable and maintainable CSS.