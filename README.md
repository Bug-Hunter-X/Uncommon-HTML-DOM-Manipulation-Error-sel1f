# Uncommon HTML DOM Manipulation Error

This repository demonstrates a subtle bug related to DOM manipulation in HTML.  The bug occurs when trying to access and modify a DOM element after it's been removed using the `remove()` method.

## Bug Description
The provided HTML code has a button that, when clicked, removes a div element from the DOM.  However, the code then attempts to modify the innerHTML of the *already removed* element, resulting in an error. This is an uncommon error as developers often forget the element is no longer part of the DOM.

## How to Reproduce
1. Clone this repository.
2. Open `bug.html` in a web browser.
3. Click the button.
4. Observe the error in your browser's console. 

## Solution
The solution involves checking if the element exists before attempting to modify it.