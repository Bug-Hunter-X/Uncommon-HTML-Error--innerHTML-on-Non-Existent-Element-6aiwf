# Uncommon HTML Bug: innerHTML on Non-Existent Element

This repository demonstrates a subtle error that can occur in HTML when using `innerHTML` to manipulate the content of an element that does not exist in the DOM.  The `bug.html` file showcases the error, while `bugSolution.html` provides a corrected version.

## The Problem

Attempting to access and modify the `innerHTML` of a non-existent element throws a JavaScript error, preventing the rest of your script from executing correctly.  This is a common problem when dealing with dynamically added elements or when there's a mismatch between the element IDs in your JavaScript and the actual HTML.

## The Solution

Always check for the existence of elements before attempting to manipulate their properties, especially `innerHTML`.  Use `getElementById` and check for `null` before proceeding.