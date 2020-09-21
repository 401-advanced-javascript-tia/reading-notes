### September 20<sup>th</sup>
## Hooks API

**Hooks let you always use functions instead of having to constantly switch between functions, classes, higher-order components, and render props.**

- Enables you to have functional components that do all the things classes do

1. Why do we not need more .html pages in a multi-page React app?
  - We don't need more than the initial index.html page because everything renders dynamically to a root area on that page. It's kind of the essence of React, that different things can render to the same area of a page based on the state of the App. Plus we can "fake" the routes (even making them change in the URL) with a Browser Router so there's no use for more than one .html page!
2. If we wanted a component to show up on every page, where would we put it and why?
  - Inside the `<BrowserRouter />`, outside a `<Route />`. Everything in the App needs to be wrapped in the Browser Router in order for the Routes to work, but if we wanted something to be on every page and not route specific we would keep it outside a Route designation.
3. What does props.children contain?
  - contains any child elements definied within the component

## Vocabulary

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| Composition | the way we comprise our App! the natural pattern of the componnt model, how we build components and possible other components from those components |
| Children / Child Components | a component that a parent component could pass data down to, via props |
| Hash Routing | uses URL hash, keeps server-side and client-side routing independent. isn't limited to a single page app but use cases are more for small, client side apps that dont need a backend  |
| Link Routing | BrowserRouter, better for bigger apps that serve backend |

- "SERVER SIDE: HashRouter uses a hash symbol in the URL, which has the effect of all subsequent URL path content being ignored in the server request (ie you send "www.mywebsite.com/#/person/john" the server gets "www.mywebsite.com". As a result the server will return the pre # URL response, and then the post # path will be handled by parsed by your client side react application."

- "CLIENT SIDE: BrowserRouter will not append the # symbol to your URL, however will create issues when you try to link to a page or reload a page. If the explicit route exists in your client react app, but not on your server, reloading and linking(anything that hits the server directly) will return 404 not found errors."


## Resources
- https://dev.to/bouhm/thinking-in-react-component-composition-fp5
- https://reactrouter.com/web/api/HashRouter
- https://stackoverflow.com/questions/51974369/hashrouter-vs-browserrouter
- https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889
- https://reactjs.org/docs/hooks-state.html
