# Reading - Custom Hooks

## Review, Research, and Discussion

1. What does a component’s lifecycle refer to?
    - "We are born, grow, and then die. Almost everything follows this cycle in its life, and React components do as well. Components are created (mounted on the DOM), grow by updating, and then die (unmount on DOM). This is referred to as a component lifecycle." -[src](https://www.freecodecamp.org/news/how-to-understand-a-components-lifecycle-methods-in-reactjs-e1a609840630/#:~:text=We%20are%20born%2C%20grow%2C%20and,to%20as%20a%20component%20lifecycle.)
1. Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
    - "useCallback is a React Hook which returns a memoized version of the callback function it is passed. This means that the function object returned from useCallback will be the same between re-renders." -[src](https://aheadcreative.co.uk/articles/when-to-use-react-usecallback/)
1. Why are functional components preferred over class components?
    - "Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks. You end up with less code. They help you to use best practices." -[src](https://djoech.medium.com/functional-vs-class-components-in-react-231e3fbd7108)
1. What is wrong with the following code?

    ``` javascript
    import React, {useState, useEffect} from 'react';

    function MyComponent(props) {
      const [count, setCount] = useState(0);

      function changeCount(e) {
        setCount(e.target.value);
      }

      let renderedItems = []

      for (let i = 0; i < count; i++) {
        useEffect( () => {
          console.log('component mount/update');
        }, [count]);

        renderedItems.push(<div key={i}>Item</div>);
      }

      return (<div>
        <input type='number' value={count} onChange={changeCount}/>
          {renderedItems}
        </div>);
    }
    ```

    - useEffect should not be in a for loop.

## Document the following Vocabulary Terms

- **state hook** - useState is a Hook that allows you to have state variables in functional components. [src](https://blog.logrocket.com/a-guide-to-usestate-in-react-ecb9952e406c/)
- **effect hook** - useEffect adds the ability to perform side effects from a function component. It serves the same purpose as componentDidMount, componentDidUpdate, and componentWillUnmount in React classes, but unified into a single API. [src](https://reactjs.org/docs/hooks-overview.html)
- **reducer hook** - An alternative to useState. useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks. [src](https://reactjs.org/docs/hooks-reference.html#usereducer)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    1. How useEffect can be implemented in different ways to simulate the different lifecycle methods used by classes.
    1. How to implement async ajax calls within a functional component.
    1. That the state hook is referring to useState and the effect hook is referring to useEffect.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. When to use useReducer and the benefits it has.
    1. When and why to use useCallback.
    1. An example of when we would use a custom hook.
1. What are you most excited about trying to implement or see how it works?
    - Using different kinds of hooks besides the state and effect hooks.

## Preparation Materials

### Authoring

- [custom hooks - all you need to know](https://www.telerik.com/blogs/everything-you-need-to-create-a-custom-react-hook)
- [async hooks](https://dev.to/vinodchauhan7/react-hooks-with-async-await-1n9g)
- [useReducer Hook](https://reactjs.org/docs/hooks-reference.html#usereducer)
- [react custom hooks](https://reactjs.org/docs/hooks-custom.html)

### Hooks Lists/Collections

- [use hooks](https://usehooks.com/)
- [hooks list](https://github.com/rehooks/awesome-react-hooks)
- [10 essential react hooks](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)
