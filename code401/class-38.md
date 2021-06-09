# Readings: Redux - Asynchronous Actions

## Review, Research, and Discussion

1. How granular should your reducers be?
    - it's generally agreed that functions should be relatively short and ideally only do one specific thing. Because of this, it's good programming practice to take pieces of code that are very long or do many different things, and break them into smaller pieces that are easier to understand. [redux](https://redux.js.org/recipes/structuring-reducers/splitting-reducer-logic)
1. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched?
    - Pro, as long as you are smart about what you're passing into the actions
1. Name a strategy for preventing the above
    - Have explicit and verbose names for actions

## Document the following Vocabulary Terms

- **store** - A store holds the whole state tree of your application. The only way to change the state inside it is to dispatch an action on it. [src](https://redux.js.org/api/store)
- **combined reducers** - As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state. The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore. The resulting reducer calls every child reducer, and gathers their results into a single state object. The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers(). [src](https://redux.js.org/api/combinereducers)

### Preparation Materials

- [async actions](https://redux.js.org/advanced/asyncactions)
- [thunk middleware](https://github.com/reduxjs/redux-thunk)
- [redux thunk](https://alligator.io/redux/redux-thunk/)
