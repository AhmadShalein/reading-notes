# Read 12: Docs for the HTML canvas Element & Chart.js:

## Canvas:
--------------------------------------------------------------------------------------------
- At first sight, a <canvas> looks like the <img> element, with the only clear difference is that it doesn’t have the src and alt attributes.
- The <canvas> element has only two attributes, width, and height.
- The canvas will initially be 300 pixels wide and 150 pixels high.
- The <canvas> element can be styled just like any normal image (margin, border, background…).
- Before we can start drawing, we need to talk about the canvas grid or coordinate space.
- There are three functions that draw rectangles on the canvas, such as:(fillRect(x, y, width, height) Draws a filled rectangle, stroke rest(x, y, width, height) Draws a rectangular outline & clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent).
- If we want to apply colors to a shape, there are two important properties we can use: fillStyle and stroke style (fillStyle = color Sets the style used when filling shapes. stroke style = color Sets the style for shapes’ outlines).
- The canvas rendering context provides two methods to render text:
1- fillText(text, x, y [, maxWidth]) Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
2- strokeText(text, x, y [, maxWidth]) Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.
