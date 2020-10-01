### Questions:

**What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?**

useEffect can be used effectively to run any async functions needed on loading and seed your store with data.

**When using a thunk/async action that dispatches the actual action, which do you export from your reducer?**

Thunk middleware works by allowing you to write action creators that return a function rather than an action.  The inner function that is exported receives the store methods dispatch and getState as parameters

*Source: https://github.com/reduxjs/redux-thun*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|thunk|functional programming technique used to delay computation|https://medium.com/fullstack-academy/thunks-in-redux-the-basics-85e538a3fe60|
|middleware|software that lies between an operating system and the applications running on it|https://azure.microsoft.com/en-us/overview/what-is-middleware/|

---

[Home](https://jchinzi.github.io/reading-notes/)