## HTML Ch. 7 - Forms

Forms come in many *forms*, including text, choices like buttons or checkboxes, submitting forms or uploading files.

Information sent from a browser to a server is sent in name/value pairs.

`<form>` elements contain form controls
The *action* attribute of the `<form>` element contains the URL for the page on the server that will receive the information with the form is submitted

Forms can be sent using one of tow methods: *get* or *post*

`<input>` is used to create values like *type*, *name* and *size* that describe the input the element will be creating

Much of this chapter describes different elements used to create forms - refer back to the text for specific examples.

**form validation** is used to ensure users enter information into a form that can be understood once submitted

---

## HTML Ch. 14 - Lists, Tables & Forms

**list-style-type** allows for formatting of markers used in `<ol>`, `<ul>` and `<li>`  Alternately, images can be used with *list-style-image*

**list-style-position** positions the marker inside or outside of the text box

- Table properties can be found on p. 337-338

- Empty cells can be formatted specifically (see p. 339)

- Text styling options can be found on p. 342

- Submit Button styling options can be found on p. 343

- Fieldset and Legend styling options can be found on p. 344

- Cursor styles can be found on p. 347

---

## JavaScript Ch. 6 - Events


**Events** are the browser's way of indicating when something has happened

**Binding** is the process of stating which event you are waiting to happen, and which element you are waiting for that event to happen upon

When an event occurs on an element it can trigger a JS function.

- Event Types are listed on p. 246-247

Events *trigger* a function or script when they are *fired* or *raised*

Event Handling involves 3 Steps

1. Select the element notes you want the script to respond to

1. Indicate which event on the selected node will trigger the response

1. State the code you want to run when the even occurs 

*event flow* describes the order in which the events that handlers/listeners are bound to fire off

- In *event bubbling*, events start at the most specific node and flow outward to the least specific

- In *event capturing*, events start at the least specific node and flow inward to the most specific

*event objects* tell information about an event when it happens, as well as the element it happened upon

*event delegation* describes delegating the job of the event listener to a parent of the element

There are event objects designed specifically to change the default behavior of an element and how the element's ancestors respond to the event.  See p. 267 for examples

**load** event is used to trigger scripts that access the contents of the page

p. 274 details *Focus* and *Blur* events

p. 276 details *Mouse* events

p. 280 details *Keyboard* events

p. 282 details *Form* events

p. 284 details *Mutation* events

---
[Home](https://jchinzi.github.io/reading-notes/)