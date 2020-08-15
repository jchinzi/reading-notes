## [Shay Howe’s Intro to RWD](https://learn.shayhowe.com/advanced-html-css/responsive-web-design/)

RWD: Responsive Web Design, or the practice of building a website suitable to work on devices of every size

- RWD has become particularly important with the rise of mobile internet usage (smart phones, etc)

*Responsive*: Reacts quickly and positively to change

*Adaptive*: Easily modified for a new purpose or situation

*Mobile*: Built separately and specifically for a mobile device

*Flexible Layout*: The practice of building the layout of a website with a flexible grid capable of dynamically resizing to any width

*Media Queries*: Provide the ability to specify different styles for individual browser and device circumstances

- Mobile First approach is one technique that targets smaller viewports (such as mobile devices) first, and then uses media queries to add styles as the viewport grows

*Flexible Media*: Addresses the need for media to be scalable, changing their size as the size of the viewport changes

To get embedded media to be fully responsive: 

- the embedded element needs to be absolutely positioned within a parent element
- the parent element needs to have a width of 100% so that it may scale based on the width of the viewport
- the parent element needs to have a height of 0 to trigger the hasLayout mechanism (IE)



---
## [All About Floats](https://css-tricks.com/all-about-floats/)

*Floated Elements remain a part of the flow of the web page*

**Float** can be set to: Left, Right, None (default) or Inherit

**Clear** can be set to: Both (most common), Left, Right, or None (default)

### Techniques for Clearing Floats

*Empty Div Method*: `<div style="clear: both;"></div>`

*Overflow Method*: Set overflow CSS property of a parent element to auto or hidden

*Easy Clearing Method*: uses CSS pseudo selector :after on a class to apply a small bit of hidden content after the parent element

---
[Home](https://jchinzi.github.io/reading-notes/)