## Article "Understanding the problem domain is the hardest part of programming"

*It is very difficult to learn more than one thing at a time*

- As a student studying software development, it is therefore very difficult to learn how to code a problem when you don't fully understand the problem when expressed in plain language

- In a professional setting, it will be much harder to build a solution if you don't fully understand the problem that you are being asked to solve

Both situations can be addressed in one of two ways: 

- Make the problem domain easier

- Get better at understanding the problem domain 

---
## JavaScript Ch. 3 - Object Literals

**property**: a variable that is part of an object

**method**: a function that is part of an object (ergo, the value of a method is *always* a function)

**key**: the unique name assigned to a value within an object.  An object cannot have two keys with the same name

  - Within an object, each key is separated from its value using a colon.  The pair is then followed by a comma

  > keyName: value,

The properties or methods of an object can be accessed using dot notation.  Properties can also be accessed using square brackets

---
## JavaScript Ch. 5 - Document Object Model

The **Document Object Model** *(DOM)* specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window.

**DOM tree** used to specify the way a browser should structure a model of a webpage (DOM)

 - begins with a *document node* that represents the entire page and corresponds to the *document object*

 - every element, attribute, and piece of text in the HTML is then represented by its own *DOM node*

**Application Programming Interface** *(API)* lets programs and scripts talk to each other

To access and update the DOM tree:

1. Locate the node that represents the element you want to work with
1. Use its text content, child elements, and attributes

**nodeList** is the collection of nodes that is returned when a method *can* return more than one node

  - A **live nodeList** is updated when a script updates the page

  -A **static nodeList** does not reflect changes made when a script updates the page

There are two possible ways to add and remove content from a DOM tree:

- The **innerHTML** Property provides new content as a string

- DOM Manipulation involves creating element and text nodes and then attaching or removing them from the DOM tree

**Cross-Site Scripting Attacks** *(XSS)* are a risk when using innerHTML, as an attacker may be able to place malicious code into the website

There are several precautions that can be taken to protect against XSS:

- Filter or Validate Input
- Limit where user content goes
  
  - Do not place user content in script tags, html comments, tag names, attributes, or CSS values 

---
[Home](https://jchinzi.github.io/reading-notes/)