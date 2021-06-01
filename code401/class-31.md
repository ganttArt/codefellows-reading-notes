# Reading: Hooks API

## Review, Research, and Discussion

1. Why do we not need more .html pages in a multi-page React app?
    - Because there are not actually multiple pages in the multi-page React app if you're using the react router. There is still just one page but different components are being displayed based on the route that is being shown.
1. If we wanted a component to show up on every page, where would we put it and why?
    - Inside the `<BrowserRouter />`, outside a `<Route />`. Every thing in a route will only show on that route. You want to be wrapping the whole app in Browser Router. If you want something to show on every page then you will put it inside the router but outside of the routes.
1. What does props.children contain?
    - Essentially, props.children is a special prop, automatically passed to every component, that can be used to render the content included between the opening and closing tags when invoking a component. These kinds of components are identified by the official documentation as “boxes”. [src](https://codeburst.io/a-complete-guide-to-props-children-in-react-c315fab74e7c)

## Document the following Vocabulary Terms

- **Composition** - React Composition is a development pattern based on React's original component model where we build components from other components using explicit defined props or the implicit children prop. 
In terms of refactoring, React composition is a pattern that can be used to break a complex component down to smaller components, and then composing those smaller components to structure and complete your application. [src](https://formidable.com/blog/2021/react-composition/)
- **Children / Child Components** - A component that is rendered within another component (it's parent).
- **Hash Routing** - When you click on a link created with react-router-hash-link it will scroll to the element on the page with the id that matches the #hash-fragment in the link. [src](https://www.npmjs.com/package/react-router-hash-link)
- **Link Routing** - Provide declarative, accessible navigation around your application. [src](https://reactrouter.com/native/api/Link)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    1. How useState is used to declare a stateful variable, the function associated with changing that state, and the starting value.
    1. How useEffect can be used to replace all of the class based component lifecycle methods.
    1. You can use useEffect multiple times, and by using the second parameter you can target the change you're checking for.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. Doubling back on useEffect and how you can create a function within it that only acts on the unmount.
    1. Creating custom hooks, and when exactly is the time when we would want to use them. What exactly is a custom hook anyway and how does it differ from just creating a function that will be called?
    1. More about just why there is such a growing preference around using hooks. I'm not quite sold yet, although I'm liking useEffect.
1. What are you most excited about trying to implement or see how it works?
    - Just going through a basic implementation of using useState and useEffect.

### Preparation Materials

- [making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)
- [the state hook](https://reactjs.org/docs/hooks-state.html)
- [hooks api](https://reactjs.org/docs/hooks-overview.html)
- [hooks api reference](https://reactjs.org/docs/hooks-reference.html)
- [effects hook](https://reactjs.org/docs/hooks-effect.html)
