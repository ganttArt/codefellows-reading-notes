# Reading: React Native

## Review, Research, and Discussion

1. Compare and Contrast Redux Toolkit with Redux “Ducks”
    - The Redux Toolkit provides a number of functions that can simplify working with Redux. It covers many standard cases by default, but can still be configured for more specific tasks. The Redux Toolkit provides a collection of libraries that are already widely used and work well together. With these libraries and the new features of the Redux Toolkit, a lot of boilerplate code can be avoided and the syntax becomes a bit clearer and easier to understand.
    - The advantages of the Redux Toolkit come at a price. You get an additional dependency through the Redux Toolkit and indirectly some dependencies through the libraries provided by the toolkit. Furthermore, the standards in the Redux Toolkit relieve the developer of some tasks. Thus, when dealing with Redux without the toolkit, knowledge gaps might arise. Especially for new developers, basic rules in working with Redux are abstracted, which might make it more difficult to gain a better understanding of Redux and the Flux pattern. [src](https://blog.codecentric.de/en/2020/02/simplifying-redux-with-the-redux-toolkit/)
1. What is the principle advantage of Redux Toolkit
    - It provides several tools that help you to "speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code." [src](https://redux.js.org/redux-toolkit/overview)
    - These tools include:
      - configureStore
      - createReduce
      - createAction
      - createSlice
      - createSelector

## Document the following Vocabulary Terms

- **redux toolkit slices** - A function that accepts an initial state, an object full of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state. [src](https://redux-toolkit.js.org/api/createSlice)
- **namespace** - a set of signs (names) that are used to identify and refer to objects of various kinds. A namespace ensures that all of a given set of objects have unique names so that they can be easily identified. Namespaces are commonly structured as hierarchies to allow reuse of names in different contexts. [src](https://en.wikipedia.org/wiki/Namespace#:~:text=In%20computing%2C%20a%20namespace%20is,they%20can%20be%20easily%20identified.)
  - Some common namespaces include the global, local, and built-in namespaces.

### Preparation Materials

- [getting started with react native](https://facebook.github.io/react-native/docs/getting-started)
- [react native basics (Tutorial)](https://facebook.github.io/react-native/docs/tutorial)
- [react native](https://facebook.github.io/react-native/)
- [expo](https://expo.io/)
- [expo snack](https://snack.expo.io/)
- [ejecting](https://docs.expo.io/versions/latest/expokit/eject)
