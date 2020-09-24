### Questions:

**Describe use cases for useMemo() and useReducer()**

- useMemo() is similar to useCallback(), except that it allows you to apply memoization to any value type rather than just functions.  It will recompute memoized values when one of the passed dependencies has changed, which helps to optimize your codes performance.

- useReducer() is similar to useState, but is preferable when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one.

*Sources:*
*https://kentcdodds.com/blog/usememo-and-usecallback*
*https://reactjs.org/docs/hooks-reference.html#usememo*
*https://reactjs.org/docs/hooks-reference.html#usereducer*

**Why do custom hooks need the use prefix?**

While custom hooks will still work if they are named differently, the convention of naming hooks with the prefix *use* is very helpful both in making your code easily readable and understandable to others (as this convention immediately signals that you are in fact using a custom hook) and in allowing React to identify custom hooks as such and therefore check for violations of rules of Hooks.

*Sources:*
*https://dev.to/sebtoombs/introduction-to-custom-react-hooks-1h37#:~:text=Custom%20hooks%20in%20React%20are,involving%20stateful%20logic)%20between%20components.&text=If%20you%20don't%20use,%2C%20%22useEffect%22%20etc).*
*https://reactjs.org/docs/hooks-custom.html*
*https://reactjs.org/docs/hooks-rules.html*

**What do custom hooks usually do?**

Custom hooks let you extract component logic into reusable functions.

*Source: https://reactjs.org/docs/hooks-custom.html*

**Using any list of custom hooks, research and name one that you think will be useful in your applications**



*Source: *

**Describe how a hook that fetches API data might work**



*Source: *

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|reducer|A pure function that takes the previous state and an action, and returns the next state|https://redux.js.org/basics/reducers|

---

[Home](https://jchinzi.github.io/reading-notes/)