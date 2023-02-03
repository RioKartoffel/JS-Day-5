# JS-Day-5
Blurry Loading

This code is a simple implementation of a "Blurry Loading" effect.

HTML:

- The HTML file starts with a declaration of the document type as HTML5 and sets the language as English.
- Then, the **`head`** section sets the title of the webpage to "Blurry Loading" and sets the character encoding as UTF-8. It also sets the viewport to the width of the device, with an initial scale of 1 and no shrink-to-fit feature.
- The **`link`** tag references an external stylesheet named "style.css".
- The body of the HTML file contains a section element with a class of "bg" and a div element with a class of "loading-text". The section element acts as a container for the background image, and the div element is used to display the loading progress.
- Finally, the body includes a reference to an external JavaScript file named "script.js".

CSS:

- The stylesheet imports a Google font named "Ubuntu" for styling the text.
- The CSS code sets the font family to "Ubuntu" for the entire document, and sets the body's display, align-items, justify-content, height, and overflow properties.
- The "bg" class sets the background image, positions it absolute and sets its width and height to be the full viewport size. It also sets the filter property to blur the image with a 0px blur radius.
- The "loading-text" class sets the font size and color of the text.

JavaScript:

- The JavaScript code uses querySelector() to select the "loading-text" div element and the "bg" section element.
- It declares a variable named "load" that is used to keep track of the loading progress, and sets its value to 0.
- It then sets an interval that calls the blurring() function every 30 milliseconds.
- The blurring() function increments the "load" variable by 1 and checks if the value is greater than 99. If it is, the interval is cleared.
- The function then updates the innerText property of the "loading-text" div element to display the current loading progress and sets its opacity using a helper function named scale().
- The function also updates the filter property of the "bg" section element to blur the background image, with the blur radius also being determined by the helper function.
- The scale() function is a simple mathematical function that maps a number from one range to another. It is used to convert the current loading progress to values used to update the opacity and blur radius.
