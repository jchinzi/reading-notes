### Questions:

**What does a component’s lifecycle refer to?**

Each React component has a lifecycle that goes through three phases:
  - Mounting
  - Updating
  - Unmounting
These phases can be monitered and the component can be manipulated depending on the phase that it is in.

*Source: https://www.w3schools.com/react/react_lifecycle.asp#:~:text=Lifecycle%20of%20Components,Mounting%2C%20Updating%2C%20and%20Unmounting.*

**Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect**

useCallback() allows you to prevent the re-creation of a function while using useEffect (which can be problematic - especially if the function that would be re-created sets off an infinite loop of re-renders)

*Source: https://medium.com/@infinitypaul/reactjs-useeffect-usecallback-simplified-91e69fb0e7a3#:~:text=useCallback()%20helps%20you%20prevent,out%20of%20the%20infinite%20loop!*

**Why are functional components preferred over class components?**

Functional components with the addition of Hooks are able to do the same work that class components are typically responsible for (state, react life cycles, etc) but in a way that is easier to maintain and test. 

*Source: https://dev.to/bryce_hao/use-functional-component-with-hooks-to-replace-class-component-14bb*

**What is wrong with the following code?**
```
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```

I'm not certain, but I think the issue may be with calling useEffect within a for loop (it should automatically re-render the page when count changes - the for loop seems like it would impede the function working correctly).

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|state hook|A Hook that lets you add React state to function components|https://reactjs.org/docs/hooks-state.html|
|effect hook|A Hook that lets you perform side effects in function components|https://reactjs.org/docs/hooks-effect.html|
|reducer hook|An alternative Hook to useState - useReducer accepts a reducer of type (state, action) => New State, and returns the current state paired with a dispatch method.  Preferable when you have complex state logic that involves multiple sub-values or when the next state depends on the prior one.|https://reactjs.org/docs/hooks-reference.html#usereducer|

---

[Home](https://jchinzi.github.io/reading-notes/)