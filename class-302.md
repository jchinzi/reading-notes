## JavaScript Ch. 7 - jQuery

*jQuery*: a JavaScript file that you include in your web pages which allows you to find elements using CSS-style selectors and then use jQuery methods

*jQuery Object* is created using the jQuery function $('element selector').methodCalled

Benefits of using jQuery:
- allows for faster selection of elements
- more accurate method of selecting elements
- more concise code
- simplifies methods for common tasks

When you select one or more elements, a *jQuery object* is returned (aka *matched set* or *jquery selection*).  Each element within that object is assigned an index number

- If a method is used to get information from a selection with more than one element, it will retrieve information from only the first element in the set

- However, if a method is used to update information and the selection holds more than one element, **all** will be updated

*implicit iteration*: the ability to update all of the elements in the jQuery selection

*chaining*: the process of placing several methods in the same selector
- most methods used to **update** the jQuery selection can be chained
- methods that **retrieve** information from the DOM or about the browser *cannot* be chained

.ready() method: checks if the browser supports the DOMContentLoaded event
- can be written in shorthand as $(function() {script});

### Common Tasks with jQuery

- Getting Element Content (p. 314)
- Updating Elements (p. 316)
- Inserting Elements (p. 318)
- Getting and Setting Attribute Values (p. 320)
- Getting and Setting CSS Properties (p. 322)
- Effects (p. 332)

*.each()* method allows one to loop through each element in a selection
- this or $(this) can be used to access the current element while using the .each() method

*.on()* method is used to handle events
- this method includes optional properties shown in square brackets:
> .on(events[, selector][, data], function(e));

---
## [6 Reasons for Pair Programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/)

Pair Programming: the practice of two developers sharing a single workstation to interactively tackle a coding task together

Driver: the programmer who is typing (the only one whose hands are on the keyboard)

Navigator: the programmer who uses their words to guide the Driver but does *not* provide any direct input to the computer

Pair Programming allows developers to practice four fundamental language skills:
- Listening: hearing and interpreting the vocabulary
- Speaking: using the correct words to communicate an idea
- Reading: understanding what written language intends to convey
- Writing: producing meaningful language from scratch

Benefits of Pair Programming:

1. Greater Efficiency
1. Engaged Collaboration
1. Learning from Fellow Students
1. Social Skills
1. Job Interview Readiness
1. Work Environment Readiness

---
[Home](https://jchinzi.github.io/reading-notes/)