### Questions:

**Can a parent component access the state of a child component?**

Parents cannot directly access the state of a child component, but the state can be accessed through the use of callback functions.

*Source: https://towardsdatascience.com/passing-data-between-react-components-parent-children-siblings-a64f89e24ecf*

**What can be passed along in a prop variable?**

Props are objects used to pass data (attributes and values) from a parent component to a child component 

*Source: https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child)*

**How can a child component “know” the state of another component?**

Components cannot proactively access the state of other components - however, you can pass a component's state to its child components as props and if components share a common ancestor, they can access the same state in a similar manner.

*Source: https://discuss.codecademy.com/t/can-a-component-access-the-state-of-another-component/394157*
*Related Content: https://towardsdatascience.com/passing-data-between-react-components-parent-children-siblings-a64f89e24ecf*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|component props|Objects that are passed to the component (similar to function parameters)|https://reactjs.org/docs/faq-state.html|
|component state|Objects that are managed within the component (similar to variables declared within a function) - this state is local to the component|https://reactjs.org/docs/faq-state.html|
|application state|Global state that can be accessed by any component within the app by hooking into it|https://teamtreehouse.com/community/what-is-the-difference-between-application-state-and-component-state-in-react|

---

[Home](https://jchinzi.github.io/reading-notes/)