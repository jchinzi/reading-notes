## HTML Ch. 4 - Links

Links to outside websites are created using the anchor element and absolute URLs, as shown below:

> `<a href="http://www.websitelink.com">Website Name</a>`

Alternately, to link to another page within the same website a shorter relative URL can be used:

> `<a href="relativeLink.html">Page Name</a>`

|Relative Link Type|Example of Relative Link|
|:--|--:|
|Same Folder|link.html|
|Child Folder|child/link.html|
|Grandchild Folder|child/grandchild/link.html|
|Parent Folder|../link.html|
|Grandparent Folder|../../link.html|

A link can also prompt the users email program to open by using the following code:

>`<a href="mailto:me@example.org">Email Me</a>`

If you want the link to automatically open in a new window rather than redirecting the current window, use the target attribute:

>`<a href="http://www.websitelink.com" target="_blank">Website Name</a>`

You an also use the id attribute to link to a specific location on a page.  ID is targeted using # (just like in CSS). 

---

## HTML Ch. 15 - Layout

(Notes focus on p.358 - p.364)

**Block-Level Elements**
- Start on a new line
- Include headings, paragraphs, and lists
- If one block-level element sits inside another block-level element, the outer box is known as the **containing** or **parent** element
  - `<div>` elements are often used for this purpose

**Inline Elements**
- Flow in between surrounding text
- Include images and style options like **bold** and *italic*

**Positioning Schemes** allow you to control the layout of the page

- **Normal Flow** sets every block-level element on a new line.  This is the default behavior

- **Relative Positioning** shifts an element from it's normal position (up, down, left or right) but does *not* affect the position of surrounding elements

- **Absolute Positioning** positions an element in relation to its containing element and takes it out of the normal flow.  Surrounding elements will ignore the space it would have taken up, and the absolutely positioned elements move as users scroll up and down the page

  - **Fixed Positioning** is a a form of absolute positioning that positions the element in relation to the browser rather than the containing element

  - **Floating** an element allows you to take that element out of normal flow and position it to the far left or right of a containing box

  - The *box offset* properties tell the browser how far from the normal edges it should be placed

  - The *z-index* property controls visibility when boxes overlap 


---

## JavaScript Ch. 3 - Functions, Methods, and Objects

**Functions** consist of a series of statements grouped together to perform a specific task.  Depending on how it is expressed, a function may be local or global in scope

- **Named Functions** can be called later in the code

- **Function Expressions** are functions that are used where an expression might normally be found.  They may be stored within a variable and cannot be processed until the interpreter gets to the statement where they are contained

  - **Methods** are like functions that are created inside of and are a part of an object
  - **Parameters** are pieces of information passed to a function that may be required to achieve a task
  - **Arguments** are values that will be used as parameters.  These may be provided as values or variables
  

**Objects** are made up of methods and properties and are used to create models of the world using data
  - **Built-In Objects** are objects that come with a browser and help create interactive web pages



---

## 6 Reasons for Pair Programming

Pair programming involves two roles: a **Driver** and a **Navigator**.

- The Driver is the person literally typing out the code - the hands on the keyboard.

- The Navigator will watch for errors, give input and make suggestions.  They may also use a second computer to research questions, etc, but will not write any of the code.

Pair Programming reinforces four key language skills: *Listening, Speaking, Reading & Writing*

**The 6 Reasons for Pair Programming**

1. Greater Efficiency
    - more likely to catch mistakes as they happen
1. Engaged Collaboration
    - keeps both programmers on track and able to ask for help
1. Learning from Fellow Students
    - exposure to different problem solving techniques and skill sets
1. Social Skills
    -improves communication skills
1. Job Interview Readiness
    - many interviews use pair programming to test how well a candidate will mesh with the existing team
1. Work Environment Readiness
    -pair programming is used in the real world - best to practice now!


---
[Home](https://jchinzi.github.io/reading-notes/)