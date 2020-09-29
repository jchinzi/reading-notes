### Questions:

**Why choose Redux instead of the Context API for global state?**

Redux is optimized for large apps with high-frequency state changes.  This is because Redux is able to selectively re-render only those components that are updated whereas Context API prompts a re-render of all components on each update of the state.

*Source: https://www.codehousegroup.com/insight-and-inspiration/tech-stream/using-redux-and-context-api*

**What is the purpose of a reducer?**

Reducers specify how the application's state changes in response to actions sent to the store

*Source: https://redux.js.org/basics/reducers*

**What does an action contain?**

Actions are objects that contain a type property (typically a string) that indicates the type of action being performed, as well as a payload (which could be any type of value)

*Source: https://github.com/redux-utilities/flux-standard-action*

**Why do we need to copy the state in a reducer?**

Redux uses shallow equality checking to compare the immutable state to the possibly-mutated state that is returned by the reducer after being passed the current state.  If the state that comes back from the reducer is different than the root state, then the altered object will be returned for rendering - otherwise, the current state object is returned.

*Source: https://redux.js.org/faq/immutable-data*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|immutable state|unchangable - a state that cannot be modified after it is created|https://en.wikipedia.org/wiki/Immutable_object.|
|time travel in redux|because Redux DevTools record dispatched actions and the state of the Redux store at every point in time, it is possible to inspect the state and 'travel back in time' to a previous application state without reloading the page or restarting the app|https://medium.com/the-web-tub/time-travel-in-react-redux-apps-using-the-redux-devtools-5e94eba5e7c0|
|action creator|functions that create actions.  the function is then passed to a dispatch function with it's argument to complete the action|https://redux.js.org/basics/actions|
|reducer|specify how the application's state changes in response to actions sent to the store|https://redux.js.org/basics/reducers|
|dispatch|dispatch functions take in the results of an action creator function and then 'dispatch' those actions|https://redux.js.org/basics/actions|

---

[Home](https://jchinzi.github.io/reading-notes/)