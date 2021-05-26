# Readings: Routing

## Review, Research, and Discussion

1. Do child components have direct access to props/state from the parent?
    - If the parent's props/state is passed down to the child.
1. When a component “wraps” another component, how does the child component’s output get rendered?

    ```javascript
    <Main>
      <Content />
    </Main>
    ```

    - `<Content/>` will be passed in as a child of main and will render wherever the child element is in it's parent/wrapper component.
    - [https://stackoverflow.com/questions/20851533/react-js-wrapping-one-component-into-another](https://stackoverflow.com/questions/20851533/react-js-wrapping-one-component-into-another)

1. Can a component, such as `<Content />`, which is a child also be used as a standalone component elsewhere in the application?
    - Sure, why not. As long as it is being passed in the props it needs.
1. What trick can a parent use to share all props with it’s children?
    - The spread operator `{...props}`. [src](https://medium.com/coding-at-dawn/how-to-pass-all-props-to-a-child-component-in-react-bded9e38bb62)

## Document the following Vocabulary Terms

- **props.children** - it is used to display whatever you include between the opening and closing tags when invoking a component [src](https://stackoverflow.com/questions/49706823/what-is-this-props-children-and-when-you-should-use-it)
- **composition** - a way to combine objects or data types into more complex ones. Common kinds of compositions are objects used in object-oriented programming, tagged unions, sets, sequences, and various graph structures. [src](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwijq9mw8ufwAhUUIDQIHSMbCd0QFjACegQIBhAD&url=https%3A%2F%2Fen.wikipedia.org%2Fwiki%2FObject_composition&usg=AOvVaw2qwou7bScVQjloxz9iWWsn)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - you can use ref's to access a child components state [src](https://www.geeksforgeeks.org/how-to-access-childs-state-in-react/)
    - If you want to send in all props from a parent component you can use the spread operator, I knew there would have to be a way to do this that was less tedious than doing each one.
    - Overall, there are just more ways to work with state and props of parent/child components than just passing functions that get those states.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Using props.children in practice.
    - Contrasting Composition and Inheritance
    - Fix for using browser router when deploying to netlify.
1. What are you most excited about trying to implement or see how it works?
    - Incorporating a spinner in RESTy using conditional rendering.

### Preparation Materials

- [browser router tutorial](https://blog.pshrmn.com/entry/simple-react-router-v4-tutorial/)
- [browser router api docs](https://reacttraining.com/react-router/web/api)

### Bookmark

- [react-if component](https://www.npmjs.com/package/react-if)
- [react testing library queries](https://testing-library.com/docs/dom-testing-library/api-queries)
- [aria roles](https://www.w3.org/TR/html-aria/)
