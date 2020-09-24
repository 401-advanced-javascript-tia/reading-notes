### September 22<sup>th</sup>
## Context API

1. Describe use cases for `useMemo()` and `useReducer()`
- **useMemo()**- used to create a memorized value, the result of the function call. Operation done once, stored in memory so it's quicker to access later.
- **useReducer()**- accepts reducer function with the app's initial state, returns the current app state and then dispatches a function. Good in a situation where you'd like to have the first loaded state of the application

2. Why do custom hooks need the use prefix?
- It is not absolutely necessary, but it's the standard convention and widely used. Makes it easy to recognize it's a hook.

3. What do custom hooks usually do?
- Let's you share logic in a functional component that wasn't possible before (unless you were using class based components)

4. Using any list of custom hooks, research and name one that you think will be useful in your applications
- **use-onClickOutside**- can track when a user clicks anywhere outside a specific component

5. Describe how a hook that fetches API data might work
- The useHook (useAjax, for ex) for that would accept a url and method, and would make the actual API calls inside the hook. It could set state with the results and it could then return the necessary things for other components to use.


## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| reducer | function that determines changes to an application's state  |



## Resources
- https://reactjs.org/docs/context.html
- https://css-tricks.com/understanding-how-reducers-are-used-in-redux/
- https://css-tricks.com/getting-to-know-the-usereducer-react-hook/
