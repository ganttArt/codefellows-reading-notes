# Readings: Redux - Combined Reducers

## Review, Research, and Discussion

1. Why choose Redux instead of the Context API for global state?
    - Because you can actually store that state between multiple files and not in one massive state object.
1. What is the purpose of a reducer?
    - It is a pure function that has a switch case. It evaluates the type of action and creates a new state based on the payload.
1. What does an action contain?
    - Type and Payload
1. Why do we need to copy the state in a reducer?
    - Because state is read-only in Redux.

## Document the following Vocabulary Terms

- **immutable state** - A state that cannot be changed in place, it is read only, like in react/redux.
- **time travel in redux** - The ability to go back in time and see what state was when different actions were taken.
- **action creator** - It's as simple as defining the action.
- **reducer** - a reducer is a pure function that takes an action and the previous state of the application and returns the new state. [src](https://www.pluralsight.com/guides/how-to-write-redux-reducer)
- **dispatch** - dispatch is a function of the Redux store. You call store.dispatch to dispatch an action. This is the only way to trigger a state change. [src](https://react-redux.js.org/using-react-redux/connect-mapdispatch) You dispatch from action to reducer.

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    1. The flow of Redux => Action -> Reducer -> Store
    1. You need to use mapDispatchToState to use access the actions in components.
    1. Dispatch is the way an action gets connected to the reducer.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. Implementing multiple reducers.
    1. How can multiple reducers can respond to the same actions?
    1. going over some valuable components in MaterialUi. That library is so dense, it would be nice to know some valuable things to use in it.
1. What are you most excited about trying to implement or see how it works?
    - Building a pretty webpage with MaterialUi.

### Preparation Materials

- [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)
- [Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)
- [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)
