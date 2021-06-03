# Reading: `<Login />` and `<Auth />`

## Review, Research, and Discussion

1. Why is the Context API useful?
    - Because you can access and change the state of a component that is deeply nested.
1. Can a component outside of a provider get its context?
    - No. The component needs to be nested inside of it's context.
1. What are some common use cases for using the Context API?
    - You have deeply nested components that need to access global state. A broad example would be something like using dark/light mode.
1. Describe “Context Hell”
    - When you have a ton of nested contexts and the code gets really messy and confusing of where you need to grab context from?

## Document the following Vocabulary Terms

- **global state** - a way to pass props from a parent component to grandchild components without having to pass the props through all child components. [src](https://www.robinwieruch.de/react-global-state-without-redux/)
- **global context** - Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. [src](https://reactjs.org/docs/context.html)
- **provider** - Every Context object comes with a Provider React component that allows consuming components to subscribe to context changes. The Provider component accepts a value prop to be passed to consuming components that are descendants of this Provider. One Provider can be connected to many consumers. Providers can be nested to override values deeper within the tree. All consumers that are descendants of a Provider will re-render whenever the Provider’s value prop changes. [src](https://reactjs.org/docs/context.html#contextprovider)
- **consumer** - A React component that subscribes to context changes. Using this component lets you subscribe to a context within a function component. [src](https://reactjs.org/docs/context.html#contextconsumer)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    1. How the terms Provider and Consumer relate to context.
    1. That Redux is a context/state management system. So it will be working in the realm of context.
    1. How context is implemented in the provider, and how we access it from the consumers.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. How will Redux change the game on state management and what does it add that is not taken care of in the context api?
    1. How to store and retrieve information in cookies with React.
    1. What is the point when you've added to many context providers.
1. What are you most excited about trying to implement or see how it works?
    - Implementing Redux as a counterpoint to using the context api.

### Preparation Materials

- [what is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)
- [react-cookies component](https://www.npmjs.com/package/react-cookies)
- [react-cookie library](https://www.npmjs.com/package/react-cookie)
