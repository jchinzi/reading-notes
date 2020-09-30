### Questions:

**How granular should your reducers be?**

Reducers should be kept as simple as possible.  One of the core rules of Redux is that reducers should *only* depend on their state and action arguments, and should only calculate and return a ndw state value based on those arguments.  While a reducer may call outside functions to perform more complex logic, they should not themselves be executing async logic, generating random values, modifying variables outside the reducer or otherwise affecting things outside the scope of the reducer function.

*Source: https://redux.js.org/style-guide/style-guide*

**Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched**

Pro if written with this intention in mind (economy of actions), but can be a con if some of those 'fires' are unintended and occurring only because of a too-common name for the action.

**Name a strategy for preventing the above**

Use names for your actions that are descriptive enough to ensure you are referencing *that* action only when it is what you have in mind and want to reference specifically.

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|store|an object used in Redux apps to hold the whole state tree of the application|https://redux.js.org/api/store|
|combined reducers|combineReducers is a helper function available in Redux whose role is to turn an object whose values are different reducing functions into a single reducing function that can be passed on to createStore|https://redux.js.org/api/combinereducers|

---

[Home](https://jchinzi.github.io/reading-notes/)