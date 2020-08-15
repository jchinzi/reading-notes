## HTML Ch. 5 - Images

Images on a webpage should:
  - Be relevant
  - Convey information
  - Convey the right mood
  - be instantly recognizable
  -Fit the color palette

To add an image, use the format:
>  `<img src="images/example.jpeg" alt="An example of alt text for an image" title="Example Title" />`

**src** tells the browser where to find the image file  
**alt** provides a text description of the image  
**title** is an attribute that provides additional information 

An image element can also include the **height** and **width** attributes to specify size

If an image is followed by a block level element, then that element will sit on a new line after the image.

If an image is placed *inside* a block level element then any text or other inline elements will flow around the image.

Three important rules for creating images are:
1. Save images in the right format (usually .jpeg, .gif, or . png)
    - Photographs are best as .jpeg
    - Illustrations and logos with flat colors are best as .gif
1. Save images at the right size (ideally, the size that you want them to appear on the website)
1. Use the correct resolution

`<figure>` elements contain images and their captions, and can contain more than one image as along as they all share the same caption

`<figcaption>` element is used to add a caption to an element

---
## HTML Ch. 11 - Color

**RGB Values** express color in terms of how much red, green and blue are used

> rgb(100,100,90)

**Hex Codes** express color in six-digit codes that represent red, green and blue.  They are expressed with a leading #

> #ee3e80

**Color Names** are predefined and recognized names in vernacular

> DarkCyan

**HSL Colors** refer to hue, saturation and lightness

   - *Hue* refers to color, expressed with a number between 0 and 360, like a color wheel 
   - *Saturation* is the amount of gray in a color, expressed as a percentage between 0 and 100
   - *Lightness* is the amount of white in a color, expressed as a percentage between 0 and 100 

**Opacity** describes whether a color is solid or not, and to what degree it can be seen through.  This attribute can be appended to an rgb or hsl value by adding a fourth number, expressed as **rgba** or **hsla** respectively

---
## HTML Ch. 12 - Text

**Typeface Terminology**

*Serif*: fonts with extra details on the ends of main strokes of the letters

*Sans-Serif*: fonts with straight ends to letters and a cleaner design

*Monospace*: Fonts where every letter is the same width

*Weight* adds emphasis and affects the amount of whitespace and contrast on a page (such as **bold** or normal)

*Style* include *Italic* and *Oblique*

*Stretch* describes how condensed or extended letters are

**font-family** property allows you to specify the typeface to be used

**font-size** property allows you to specify the size of the font in pixels, percentages (as compared to the default of 16px) or ems (the width of the letter 'm')

**@font-face** can be used to introduce a font that may not be installed normally - if a user does not have the font, this will download the necessary font onto the users' machine.  It includes the attributes *font-family*, *src* and *format*

**text-transform** can be used to change the case of text into *UPPERCASE*, *lowercase* or *Capitalize*

**text-decoration** includes several options:
  
  - *none* removes all decoration
  - *underline* adds a line beneath the text
  - *overline* adds a line above the text
  - *line-through* adds a line through the text
  - *blink* animates text to make it flash on and off (this is not recommended as many find it annoying)

**line-height** sets the height of the entire line of text

**letter-spacing** & **word-spacing** are similarly self explanatory

**text-align** can be set to *left*, *right* *center* or *justify*

**vertical-align** is used with inline elements to perform a task similar to the HTML *align* attribute used on `<img>` elements.  It can be set to:

  - *baseline*
  - *sub*
  - *super*
  - *top*
  - *text-top*
  - *middle*
  - *bottom*
  - *text-bottom*

**text-indent** affects only the first line of text within an element

**text-shadow** creates a drop shadow and can take 3 values:

  - how far to the left or right the shadow should fall
  - the distance to the top or bottom that the shadow should fall
  - the amount of blur applied (optional)
  - a fourth value indicating color can also be added

***Pseudo-Elements*** (specified at the end of a selector)
- :first-letter
- :first-line
- :link (ie unvisited links)
- :visited (ie visited links)
- :hover
- :active
- :focus

|Attribute Selector|Format|Meaning|
|:--|:-:|--:|
|Existence|[ ]|Matches a specific attribute (whatever it's value)|
|Equality|[=]|Matches a specific attribute with a specific value|
|Space|[~=]|Matches a specific attribute whose value appears in a space-separated list of words|
|Prefix|[^=]|Matches a specific attribute whose value begins with a specific string|
|Substring|[*=]|Matches a specific attribute whose value contains a specific substring|
|Suffix|[$=]|Matches a specific attribute whose value ends with a specific string|







---
[Home](https://jchinzi.github.io/reading-notes/)