### Questions:

**What does a component’s lifecycle refer to?**



*Source: *

**Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect**



*Source: *

**Why are functional components preferred over class components?**



*Source: *

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



*Source: *

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|state hook|||
|effect hook|||
|reducer hook|||

---

[Home](https://jchinzi.github.io/reading-notes/)