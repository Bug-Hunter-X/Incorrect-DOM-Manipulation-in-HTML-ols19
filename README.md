# Incorrect DOM Manipulation in HTML

This repository demonstrates a common mistake in JavaScript when working with the HTML DOM (Document Object Model).

The `bug.html` file contains code that incorrectly attempts to access and modify the content of an HTML element. The `bugSolution.html` file provides the correct approach. This error occurs because the `getElementById` method returns a DOM element and not a string representation. Attempts to directly manipulate the properties will fail. To access the innerHTML, use the `.innerHTML` property after retrieving the element using `getElementById`. 

## Bug Description
The bug arises from attempting to access and modify the content of an HTML element without properly utilizing the methods provided by the Document Object Model (DOM). Using the id as a property or direct manipulation will return errors.  The correct way to obtain the HTML content is with `document.getElementById("myDiv").innerHTML` and changes are applied similarly. 