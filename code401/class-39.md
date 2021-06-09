# Readings: Redux - Additional Topics

## Review, Research, and Discussion

1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
    - The most 'redux-like' way of handling the pre-loading of data would be to fire off the asynchronous action in the lifecycle method (probably componentWillMount) of a Higher Order Component that wraps your app. However, you will not use the results of the API call directly in that component - it needs to be handled with a reducer that puts it into your app store. This will require you to use some sort of a thunk middleware to handle the asynchronous action. Then you will use mapStateToProps to simply pass it down to the component that renders the data. [src](https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux)
1. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
    - You export your action creator. [src](https://read.reduxbook.com/markdown/part1/04-action-creators.html)

## Document the following Vocabulary Terms

- **middleware** - Middleware is software that lies between an operating system and the applications running on it. Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications. [src](https://azure.microsoft.com/en-us/overview/what-is-middleware/#:~:text=Middleware%20is%20software%20that%20lies,data%20management%20for%20distributed%20applications.)
- **thunk** - Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests. [src](https://github.com/reduxjs/redux-thunk)

### Preparation Materials

- [Redux Toolkit (RTK)](https://redux-toolkit.js.org/)
  - [Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

#### Alternative State Managers

- [MobX](https://mobx.js.org/getting-started.html)
- [HookState](https://hookstate.js.org/)
