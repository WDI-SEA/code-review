# Code Guide

Listed below are some things to think about when looking through code:

### General

* Is the code DRY? What are some areas that could benefit from modularization or functions?
* Is the code formatted correctly? Indentation and spacing is important.
* What functions and variables are defined in the code?
* Are functions and variables named appropriately? Semantic naming is important.
* Are variables and functions scoped properly? Scope should be limited where possible.
* Can variables be organized in a better fashion? Examples include using objects and arrays.

### HTML

* Is the HTML document valid?
  - `<!DOCTYPE html>`
  - `<html>` tags
  - `<head>` tags
  - `<title>` tags
  - `<body>` tags
* Are CSS files linked in the head?
* Are JS files linked near the end of the body? (head if appropriate)
* If the site is reponsive, is the viewport meta tag being included in the file?
* Do form inputs have labels?

### CSS

* Are selectors clear to read and semantic?
* Are IDs being used sparingly?

### Vanilla JS/jQuery

* Making sure code that depends on the DOM is wrapped in the following:
  ```js
  // vanilla JS
  document.addEventListener('DOMContentLoaded', function() {
    // code here
  });

  // or... jQuery
  $(document).ready(function() {
    // code here
  });
  ```
