# Uncommon HTML Bug: Incorrect CSS Property Access and innerText vs. textContent

This repository demonstrates two uncommon bugs in HTML:

1. **Incorrect CSS Property Access:** The example shows an attempt to directly access a CSS property using `document.getElementById("myDiv").style.background-color`. This might not work consistently across browsers because it only returns the inline style, and not the computed style from CSS rules.  The correct way to access this is demonstrated using `window.getComputedStyle()`. 
2. **innerText vs. textContent:** The example highlights the difference between `innerText` and `textContent`.  `innerText` preserves extra spaces and line breaks, while `textContent` does not. This can lead to unexpected rendering results if not handled appropriately.

The solution demonstrates the correct ways to access CSS properties and illustrates the behavior of `innerText` versus `textContent`.  This illustrates the importance of understanding the subtle differences in how these features work to avoid unexpected behavior.