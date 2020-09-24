### Questions:

**Why is the Context API useful?**

Context provides a way to pass data through the componenet tree without having to pass props down manually at every level.

*Source: https://reactjs.org/docs/context.html*

**Can a component outside of a provider get its context?**

A Provider component works by allowing consuming components to subscribe to context changes.  All consumers that are descendants of a Provider will then re-render whenever the Provider's value prop changes.

*Source: https://reactjs.org/docs/context.html#contextprovider*

**What are some common use cases for using the Context API?**

Context is ideal for larger apps where nested components require access to a state that the is not necessarily used by all parent components, as it removes the necessity for every parent to pass props along to their children and risk creating a bug if that prop is ever passed incorrectly.

**Describe “Context Hell”**

Because Context avoids prop drilling by creating global variables, it becomes possible for those global variables to become mutated and tracing the source of an unwanted mutation can be very difficult.

*Source: https://codethrasher.com/post/2019-08-02-the-path-to-hell/*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|global state|A state that is available to and influences all levels of an environment||
|global context|React context is designed to share data that can be considered 'global' for a tree of React components|https://reactjs.org/docs/context.html|
|provider|The Provider React component allows consuming components to subscribe to context changes.  One Provider can be connected to many consumers|https://reactjs.org/docs/context.html#contextprovider|
|consumer|The Consumer React component subscribes to context changes.  This allows you to subscribe to a context within a function.|https://reactjs.org/docs/context.html#contextconsumer|

---

[Home](https://jchinzi.github.io/reading-notes/)