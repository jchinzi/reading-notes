### Questions:

**Name 3 advantages to Test Driven Development**

- TDD forces the developer to think through what the code *ought* to be doing because they are writing a test to check for specific returns or behavior.
- TDD makes debugging easier by catching bugs early in the process.  Tests can also be written to check for specific bugs.
- TDD can be an enjoyable part of coding once you learn the basics

*Source: https://jrsinclair.com/articles/2016/gentle-introduction-to-javascript-tdd-intro/*

**In what case would you need to use beforeEach() or afterEach() in a test suite?**

These are helper functions meant to be used when there is work that needs to be done repeatedly for multiple tests, such as initializing or clearing a database that a test will interact with.  beforeEach() and afterEach() can also handle asynchronous code by taking a 'done' parameter or returning a promise.

*Source: https://jestjs.io/docs/en/setup-teardown*

**What is one downside of Test Driven Development**

There is a fairly significant upfront time commitment to TDD - that time commitment usually begins to taper off over time because the resulting code is cleaner and easier to build on.  However, for small projects or code that is unlikely to be reusued or maintained then TDD may not be worth the time investment.

*Source: http://www.letscodejavascript.com/*

**What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

Classes allow for inheritance by extending classes and using super();

**Name a use case for a static method**

Static methods are called without instantiating their class and are not callable when the class is instantiated.  They are meant to provide class-specific methods for object-oriented programming.

*Source: https://medium.com/@yyang0903/static-objects-static-methods-in-es6-1c026dbb8bb1#:~:text=Static%20methods%20in%20Javascript%20are,static%20inside%20the%20class%20declaration.&text=As%20MDN%20describes%20it%2C%20%E2%80%9CStatic,when%20the%20class%20is%20instantiated.*

**Write an example of a Higher Order function and describe the use case it solves**
```
const mapTwoToThe = (arr) => {
  let newArr = arr.map(val =>
    Math.pow(2, val));
  return newArr;
};
````
Map is a higher order function that iterates over an array applies a given function to each element of that array, returning a new array.  In this case, the returned array will be an array of values that have been raised to the power of 2.
*Code pulled from 301 Code Challenges - Map*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|functional programming|The process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects|https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0|
|pure function|A function that A) always returns the same results if the same arguments are passed in and B) does not produce any observable side effects|https://medium.com/@jamesjefferyuk/javascript-what-are-pure-functions-4d4d5392d49c|
|higher-order function|A function that operates on other functions, either by taking them as arguments or by returning them|https://eloquentjavascript.net/05_higher_order.html|
|immutable state|A state in which nothing can be mutated or changed|https://softwareengineering.stackexchange.com/questions/235558/what-is-state-mutable-state-and-immutable-state|
|object|A collection of properties|https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects#:~:text=JavaScript%20is%20designed%20on%20a,is%20known%20as%20a%20method.|
|object-oriented programming (OOP)|Programming in which one uses objects to model real world things that one wants to represent inside the program and/or provide a simple way to access functionality that would otherwise be hard or impossible to make use of.|https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Object-oriented_JS|
|class|A specific type of function - class syntax has two components: class expressions and class declarations|https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes|
|prototype|A type of object to which additional properties can be attached to it which will be shared across all the instances of it's constructor function|https://www.tutorialsteacher.com/javascript/prototype-in-javascript|
|super|A keyword used to access and call functions on an objects parents|https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/super#:~:text=The%20super%20keyword%20is%20used,both%20classes%20and%20object%20literals.|
|inheritance|The method by which methods from a base class are copied to a derived class|https://www.tutorialsteacher.com/javascript/inheritance-in-javascript
|constructor|A function that creates an instance of a class which is typically called an object.  Uses the 'new' keyword|https://www.educative.io/edpresso/what-is-a-constructor-in-javascript|
|instance|A particular version of a class||
|context|The value of 'this' in the code that you are running|https://www.youtube.com/watch?v=fjJoX9F_F5g|
|this|A keyword whose value is dependent upon it's parent object (or the global object, if it is not within a more specific object)|https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this|
|Test Driven Development (TDD)|A technique for ensuring that your code does what you think it does by comparing the results of a test against the results of the production code.|http://www.letscodejavascript.com/|
|Jest|A JavaScript testing framework|https://jestjs.io/|
|Continuous Integration (CI)|A development practice that requires developers to integrate code into a shared reopository several times a day - each check-in is then verified by an automated build, allowing teams to detect problems early|https://www.thoughtworks.com/continuous-integration|
|unit test|A software testing technique by means of which individual units of software are tested to determine whether they are suitable for use or not|https://www.geeksforgeeks.org/unit-testing-software-testing/|

---

[Home](https://jchinzi.github.io/reading-notes/)