### September 13<sup>th</sup>
## Component Based UI

1. Name 5 Javascript UI Frameworks (other than React)
- Indeed there are several other Javascript UI frameworks other than React! To name a few: Vue, Angular, Ember, Preact, Svelte. 
2. What’s the difference between a framework and a library?
- A library has set functions already outlined that an app can call to perform a task, while a framework defines how an app is designed. A framework will call on the app code vs the other way around like in a library. 


## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| Rendering | in React this only happens when necessary because its only thinking about how UI should look at any given moment |
| Templating | React uses JSX which is similar to a templating language but "comes with full power of Javascript"|
| State | where your app is at any moment in time. as it relates to React, there is a built in state object and when the state object changes, that specific component re-renders  |
| JSX | JavaScript Extension- allows you to write markup directly in javascript. some differences (like className="" instead of class="", for ex)|


## Notes from lecture
- **Instead of artificially separating technologies by putting markup and logic in separate files, React separates concerns with loosely coupled units called “components” that contain both**
- Our job as app programmer is to manage state, let React take care of the view of that
- npx create-react-app _____
- everything happens in the one div id="root" in index.html
- **functional component**'s job is to return something React can render
  - use a functional component when you can! otherwise, use a class
- **class** 
  - needs to extend a very important super constructor
    - class ____ **extends React.Component**
  - needs to have a render() method in it
  - needs to call super 


### Resources
- https://reactjs.org/docs/hello-world.html
- https://www.lambdatest.com/blog/best-javascript-framework-2020/
- https://blog.newrelic.com/engineering/best-javascript-libraries-frameworks/



