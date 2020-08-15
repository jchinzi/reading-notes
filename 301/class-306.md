## [An Introduction to Node.js](https://www.sitepoint.com/an-introduction-to-node-js/)

Per the project's homepage:
> Node.js is a JavaScript runtime built on Chrome's V8 JavaScript engine

According to Stack Overflow:
>Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google's V8 JavaScript engine and libuv library.

At it's simplest, this all means that Node.js is a program we can use to execute JavaScript on our computers (a JavaScript runtime).

Node comes bundled with a package manager called npm.  
- Npm is also the world's largest software registry with over 1,000,000 packages of JS code available to download.

Together, Node and npm are used to build various tools - npm installs them and then Node runs them.

**The Node.js Execution Model**

Whereas traditional servers spawns a new thread for every request (which can cause systems to become sluggish or crash), Node.js is single-threaded and event-driven, meaning it can implement asynchronous behavior.

**Advantages of Node.js**

- Allows for the server and the client to both share one language - JavaScript - which is iteslf a ubiquitous language.
- Node is able to speak JSON, which means that data can flow neatly between the browser, server, and database without needing to be reformatted

---
[Home](https://jchinzi.github.io/reading-notes/)