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



---
[Home](https://jchinzi.github.io/reading-notes/)