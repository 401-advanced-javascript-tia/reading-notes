### September 28<sup>th</sup>
## Redux - Combined Reducers

1. Why choose Redux instead of the Context API for global state?
- As an application scales it is easier to control individual pieces of state by using Redux. Its an easier way to drill into props.

2. What is the purpose of a reducer?
- A reducer is a function that determines changes to an application's state. It grabs the action, deconstructs it, and uses it to determine the change and what to do with it. 

3. What does an action contain?
- An action should contain a type and a payload, and while these names are set in stone it's the naming convention and should be stuck to. You can peel off the type and payload from the action object and use them to initiate dispatches. 

4. Why do we need to copy the state in a reducer?
- Because we want to always be dealing with unmutated state, so we need to make a copy of it with the new thing that we are altering in the relevant part of the reducer. 

## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| immutable state | required by Redux |
| time travel in redux  | what is possible when you use the redux dev tools! you can trace back through the state changes, very neat |
| action creator  | the reducer deals with the action |
| reducer  | function that determines changes to an app's state  |
| dispatch  | the dispatch event that can be listened to and initiate action |



## Resources
- https://css-tricks.com/understanding-how-reducers-are-used-in-redux/
- https://redux.js.org/recipes/structuring-reducers/using-combinereducers/
- https://redux.js.org/api/combinereducers/