### Questions:

**Given the examples of front-end events such as button click, window resize, form submit, etc, what are some examples of back-end events?**

Backend events may include interacting with a database (CRUD operations) or a user logging into/out of a site.

**Why are events sometimes better than asynchronous actions with callbacks?**

Calling listeners synchronously in the order in which they are registered ensures the proper sequencing of events and helps avoid race conditions and logic errors.

*Source: https://nodejs.org/api/events.html*

**What does an EventEmitter instance do?**

An EventEmitter is an object that exposes an eventEmitter.on() function that allows one or more functions to be attached to named events emitted by objects.  When an eventEmitter object emits an event, all the functions attached to that specific event are called synchronously and any values returned by the called listeners are ignored.

*Source: https://nodejs.org/api/events.html*

**When is a program’s call stack, event queue, and event loop active?**

As a program is run, functions are sent to the call stack in the order that they are encountered.  They are then handled - in order - with the exception of asynchronous functions that are sent to a callback queue to await execution.  The Event Loop is what processes these functions , beginning with the call stack and then checking the callback queue if the call stack is fully executed. 

*Source: https://medium.com/@Rahulx1/understanding-event-loop-call-stack-event-job-queue-in-javascript-63dcd2c71ecd#:~:text=Event%20Loop%3A%20Then%20comes%20the,Main%20Stack%20for%20the%20execution.*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|Observer Pattern|As opposed to the MVC implementation, where the model updates the view through the controller, with the Observer Pattern we make the model into an 'observable', and a view into an 'observer'.  When the 'observable' is changed, it notifies the 'observer' of its state and the 'observer' can react to that change - making the data flow unidirectional.|https://medium.com/@patrickackerman/the-observer-pattern-with-vanilla-javascript-8f85ea05eaa8|
|Listener|A function that 'listens' for an event and then initiates the function when the event occurs|https://idratherbewriting.com/events-and-listeners-javascript/|
|Event Handler|Functions used to handle - and verify - user input, user actions, and browser actions|https://www.w3schools.com/js/js_events.asp|
|Event Driven Programming|Programming built on the idea of there being at least one 'subject' and one 'observer' that will drive actions|https://www.valentinog.com/blog/event/|
|Event Loop|The flow of actions that occur under the hood while running JS asynchronous programs|https://www.educative.io/edpresso/what-is-an-event-loop-in-javascript|
|Event Queue|Responsible for sending new functions to the call stack for processing.  The event queue follows the queue data structure to maintain the correct sequence in which all operations should be sent for execution|https://www.educative.io/edpresso/what-is-an-event-loop-in-javascript|
|Call Stack|Responsible for keeping track of all operations in line to be executed.  Follows the FILO principle - hence the 'stack' model.|https://www.educative.io/edpresso/what-is-an-event-loop-in-javascript|
|Emit/Raise/Trigger|The .emit() method is used to trigger an event|https://nodejs.org/api/events.html|
|Subscribe|The subscriber function defines how to obtain or generate values or messages to be published|https://angular.io/guide/observables|
|database|An organized collection of structured information, or data, typically stored electronically in a computer system|https://www.oracle.com/database/what-is-database.html#:~:text=A%20database%20is%20an%20organized,database%20management%20system%20(DBMS).|

---

[Home](https://jchinzi.github.io/reading-notes/)