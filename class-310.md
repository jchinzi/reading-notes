## [The Call Stack defined on MDN](https://developer.mozilla.org/en-US/docs/Glossary/Call_stack)

**call stack**: mechanism for an interpreter to keep track of its place in a script that calls multiple functions
- what function is currently being run
- what functions are called within that function

Call stacks begin empty, add functions as they are called, and once each function has executed all of its code it is automatically removed from the call stack.  This process will continue till the call stack is completely empty again.

---

## [Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

The call stack is inherently synchronous, executing functions one at at time, top to bottom.

**LIFO**: Last In, First Out, meaning that the last function pushed into the stack is the first to be returned

- When a function is called and pushed into the stack it forms a *stack frame*, which is a memory location in the stack
- When the function returns and leaves the stack, the memory is cleared

**Stack Overflow** occurs when there is a recursive function with no exit point

---

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

**Types of Error Messages:**

- *Reference Errors* (common with undeclared variables)
- *Syntax Errors*
- *Range Errors* (common with invalid length values)
- *Type Errors* (common when mistakenly accessing properties of undefined type variables)

**Tools for Debugging**

- console.log();
- debugger statements
- try...catch

---

[Home](https://jchinzi.github.io/reading-notes/)