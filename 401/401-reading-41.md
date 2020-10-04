### October 4<sup>th</sup>
## React Native

1. Compare and Contrast Redux Toolkit with Redux “Ducks”
- The idea behind "Ducks" is to create a file structure that is scalable and easy to follow. Ducks file structure says that the Redux components (reducers, actions, types) live with the components they're dealing with. The Redux Toolkit deals more with the simplification of writing those Redux components themselves.

2. What is the principle advantage of Redux Toolkit?
- It seems that the main advantage of Redux Toolkit is that it includes utility functions that simplify the most common Redux use cases for you (store setup, defining reducers, etc)

## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| redux toolkit slices  | function that accepts initial state, object full of reducer functions, and a *slice name* and automatically generates action creators and action types that correspond to the reducers and state |
| namespace  | used for the purpose of grouping symbols and identifiers are a particular functionality and to avoid name collisions between multiple identifiers that share the same name|


## Resources
- https://reactnative.dev/docs/getting-started
- https://medium.com/@thinkwik/react-native-what-is-it-and-why-is-it-used-b132c3581df
- https://redux-toolkit.js.org/api/createSlice#:~:text=A%20function%20that%20accepts%20an,approach%20for%20writing%20Redux%20logic.
- https://en.wikipedia.org/wiki/Namespace