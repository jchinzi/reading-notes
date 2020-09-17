### Questions:

**Do child components have direct access to props/state from the parent?**

Parents have to share their states (and any other information they wish to pass along) by passing props to their child components.

**When a component “wraps” another component, how does the child component’s output get rendered?**

Wrapped components receive all the props of the container - along with any additional props that may be passed - and is rendered based on those props.

*Source: https://reactjs.org/docs/higher-order-components.html*

**Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?**

Yes - components are modular, reusable pieces of code that can be rendered multiple times if need be.

**What trick can a parent use to share all props with it’s children**

A spread operator can be used as a cleaner way to pass all props without having to retype them.  For example:

```
const IntermediateComponent = (props) => {
  return (
    <ChildComponent prop1={props.prop1} prop2={props.prop2} />
  )
}
```
can instead be written as
```
const IntermediateComponent = (props) => {
  return (
    <ChildComponent {...props} />
  )
}
```

*Source: https://flaviocopes.com/react-pass-props-to-children/*

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|props.children|Used to display whatever you include between the opening and closing tags when invoking a component|https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891|
|composition|A natural pattern of the component model, or how we build components from other components|https://dev.to/bouhm/thinking-in-react-component-composition-fp5#:~:text=What%20is%20Composition%3F,in%20building%20many%20other%20components.|

---

[Home](https://jchinzi.github.io/reading-notes/)