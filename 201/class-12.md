## [Charts.js](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)

[Chart.js](https://www.chartjs.org/docs/latest/) is a JavaScript plugin used to draw a graph onto a page.  The script can be linked to your HTML just like any other JS file.

`<canvas>` tags are used to create a canvas element where we can then draw a chart

This plugin can be used to create various types of charts, including line graphs, pie charts and bar charts

---
## [Basic Usage of Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Basic_usage)

The `<canvas>` element has only two attributes: *width* and *height* and can be styled with CSS like an image.

Fallback content should also be provided inside the `<canvas>` element so that browsers that cannot support the tag can display the fallback content instead

The *getContext()* method takes one parameter - the type of context - and is used to obtain the rendering context and its drawing functions



---
## [Drawing Shapes with Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)

The canvas of a grid is described in units of pixels and begins at the top left corner (0,0)

`<canvas>` supports two primitive shapes: rectangles and paths

Rectangles take the parameters (x, y, width, height), with x and y specifying the position on the canvas of the top-left corner of the rectangle

Paths are stored as a list of sub-paths which together will form a shape - the list is reset every time the method is called

Arcs can be drawn using an arc() or arcTo() method that takes in starting points as well as a radius, angle and direction

Bezier and Quadratic curves can be used to draw more organic shapes

---
## [Applying Styles and Colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)

*fillStyle* can be used to set color in filled shapes 

*strokeStyle* can be used to set color for shapes' outlines

*globalAlpha* can be set to a transparencyValue between 0.0 (fully transparent) and 1.0 (fully opaque)

Line Style and Line Width can also be adjusted by adjusting the necessary properties

*lineCap* property defines how the end points of lines are drawn (either butt, round, or square)

Similarly, the *lineJoin* property defines how connecting segments are joined (either round, bevel, or miter)

Linear and Radial gradients allow for a gradual change of color

Shadows can be set with an x and y offset, a blur and a color

---
## [Drawing Text](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)

Text can be rendered using fillText or strokeText.  Both take the parameters (text, x, y, [, maxWidth])

This text can then be adjusted using properties like font, textAlign, textBaseline, and direction (similar to CSS)

measureText() allows one to actually measure the text width in pixels when drawn in the current style

---
[Home](https://jchinzi.github.io/reading-notes/)