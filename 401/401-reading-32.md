### September 22<sup>nd</sup>
## Custom Hooks


1. What does a component’s lifecycle refer to?
- The compenets lifecycle refers to the three phases of a component that you can monitor and manipulate- mounting, updating, unmounting.

2. Why do you sometimes need to “wrap” functions in `useCallback` when called from within `useEffect`
- It is used to allow you to prevent the re-creation of a function inside a functional component (because they're recreated every time the component rebuilds).

3. Why are functional components preferred over class components?
- Less code! Easier to read and understand.

4. What is wrong with the following code?
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
- the useEffect hook doesn't need to be inside the for loop, because there will never be more than one count item because it's getting clobbered each time it changes, in the changeCount function
- instead, use the spread operator to add to it

## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| state hook | the way to affect state without using a class and setState. returns a pair which is the current state value and the function to update it |
| effect hook | allows you to handle side side effects in the functional components |
| reducer hook | accepts a reducer function with the app initial state, returns the current app state and then dispatches a function|


## Resources
- https://www.telerik.com/kendo-react-ui/react-hooks-guide/#toc-custom-react-hooks
- https://reactjs.org/docs/react-component.html
- https://medium.com/@infinitypaul/reactjs-useeffect-usecallback-simplified-91e69fb0e7a3#:~:text=useCallback()%20helps%20you%20prevent,created%20if%20its%20dependencies%20changed
- https://reactjs.org/docs/hooks-overview.html

