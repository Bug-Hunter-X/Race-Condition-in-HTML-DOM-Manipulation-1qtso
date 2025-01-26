# Uncommon HTML Bug: Race Condition in DOM Manipulation

This repository demonstrates a subtle race condition that can occur when manipulating the DOM in HTML.  The JavaScript code attempts to access and modify a DOM element before the browser has finished rendering it.  This can lead to unpredictable results, such as the modifications not taking effect or JavaScript errors.

## Bug Description

The `bug.html` file contains a simple HTML structure with a `div` element.  The JavaScript code tries to change the color of this `div` before the browser has fully rendered the element.  This often leads to the style change being ignored.

## Solution

The `bugSolution.html` file demonstrates the solution using the `DOMContentLoaded` event.  This ensures the JavaScript code executes only after the entire HTML document has been parsed and the DOM is ready. 