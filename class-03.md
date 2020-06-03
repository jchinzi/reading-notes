## HTML Ch. 3 - Lists

|Term|Tag|Definition|
|:--|:-:|--:|
|Ordered List|`<ol>`|List where each item is numbered|
|Unordered List|`<ul>`|List where each item begins with a bullet point|
|List Item|`<li>`|Each item in an ordered and unordered list|
|Definition List|`<dl>`|List made up of a set of terms along with definitions for each term|
|Defined Term|`<dt>`|The term being defined|
|Definition|`<dd>`|The definition|

- Lists can be nested by putting a second ordered or unordered list inside a list item, thereby creating a sub-list.

---

## HTML Ch. 13 - Boxes

CSS treats each HTML element as if it has its own box, and allows you to control the dimensions and properties of that box

Boxes default to a size just big enough to contain their contents.  However, this can be changed using height and width properties

- *height* and *width* can be defined in terms of pixels, percentages, or ems

  - Percentages refer to the size relative to the browser or containing box (if applicable)
  - Ems refer to the size of the text within the box

  - *min-width* and *max-width* properties dictate the minimum and maximum size a box can be displayed when the browser window size is changed  
  - A similar result can be achieved with *min-height* and *max-height*

- *overflow* tells the browser what to do if the contents of a box are larger than the box

  - *hidden* will hide any additional content

  - *scroll* will add a scrollbar so users can access additional content by scrolling down

*border* separates the edge of one box from another

  - *border-width* can be noted in pixels or using the key words *thin*, *medium* or *thick*
  - there are many border styles available, including *solid*, *dashed*, and *inset*
  - *border-color* can be specified using RGB values, hexcodes, or CSS color names
  - the formatting of the four sides of the border can be set individually

*margin* separates adjacent boxes from one another, usually in terms of pixels

  - if one box sits on top of another, margins are collapsed and the larger of the two margins will be used, disregarding the smaller one

*padding* creates space between the *border* and the contents of the box, usually in terms of pixels

> In order to center content, set a *width* so that the box will not fill the full page and then set *left-margin* and *right-margin* to auto

*display* can be used to change inline elements into block-level elements(or vice versa)
  - *inline-block* will cause a block-level element to flow like an inline element but retain other normal block features 
  - *none* hides an element from rendering on the webpage

> *visibility* can be set to *hidden* or *visible* - however remember that hidden elements will leave a blank space, unlike *display: none*

*border-image* and *box-shadow* can be used to add decorative elements to the edge of your box

Adjusting the *border-radius* allows for rounded corners on your box

---

## JavaScript Ch. 4 - Decisions and Loops

|Term|Definition|
|:--|--:|
|Switch Statement|Indicates multiple possible code options that may run depending on the **switch value** assigned.  Once one of the codes is run, a **break** statement prevents any further **switch statements** from running|
|Type Coercion|When JavaScript converts a data type in an attempt to complete an operation|
|Unary Operator|An operator that returns a result with just one operand|

<p style="text-align: center;">Loops check a condition.  If it returns true, a code block will run.  Then the condition will be checked again and if it still returns true, the code block will run again.  This will continue until the condition returns false.</p>

|Loop Type|Description|
|:--|--:|
|For|Runs code **for** a specific number of times, often by using a counter.|
|While|Code will run for as long as the specified condition is true - useful when you don't know how many times the code will need to run.|
|Do While|Similar to *while* loops, **except that** it will always run the statement inside the curly braces at least once, *even if the condition evaluates to false*.

|Term|Definition|
|:--|--:|
|break|Causes the termination of the loop and tells the interpreter to go onto the next statement of code outside the loop.|
|continue|Tells the interpreter to continue with the current iteration, and then check the condition again|


---
[Home](https://jchinzi.github.io/reading-notes/)