# Reading: Context API

## Review, Research, and Discussion

1. Describe use cases for useMemo() and useReducer()
    - useMemo calls a function when dependencies change, and memoizes (remembers) the result of the function between renders. You want to use useMemo to save yourself from rerunning an expensive calculation to generate a new value. Use when:
        - You're noticing a component's render is frustratingly slow, and you're passing a calculation to an unknowable number of children, such as when rendering children using Array.map()
        - Your app often becomes unresponsive because you're fetching a large amount of data, and having to transform it into a usable format
        - [src - https://maxrozen.com/understanding-when-use-usememo](https://maxrozen.com/understanding-when-use-usememo)
    - useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks. [src](https://reactjs.org/docs/hooks-reference.html#:~:text=useReducer%20is%20usually%20preferable%20to,dispatch%20down%20instead%20of%20callbacks.)
1. Why do custom hooks need the use prefix?
    -  This convention is very important. Without it, we wouldn’t be able to automatically check for violations of Rules of Hooks because we couldn’t tell if a certain function contains calls to Hooks inside of it. [src](https://reactjs.org/docs/hooks-custom.html#extracting-a-custom-hook)
1. What do custom hooks usually do?
    - Custom hooks allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks. [src](https://www.wix.engineering/post/custom-react-hook-when-software-design-meets-react-hooks#:~:text=Custom%20hooks%20allow%20us%20to,use%20cases%20to%20reusable%20hooks.)
1. Using any list of custom hooks, research and name one that you think will be useful in your applications
    - useForm: this is very handy for handling the logic of storing the inputs that a user is typing into a form... no matter what inputs are going to be.
1. Describe how a hook that fetches API data might work
    - You would create a hook that makes the api calls, what you're passing into it is the url and potentially the item id if you're targeting a specific piece of data in the db.

## Document the following Vocabulary Terms

- **reducer** - a function that determines changes to an application's state. It uses the action it receives to determine this change. [src](https://css-tricks.com/understanding-how-reducers-are-used-in-redux/)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    1. useMemo is a hook designed to help with memoization and thereby optimization of your webpage.
    1. useReducer is an alternative to useState, and will be used when what is in state is on the more complex side.
    1. How custom hooks like useForm or useAjax are going to help separate the application logic into reusable chunks and also make each component more readable.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. How Redux relates to useReducer. I saw some sort of comparision or linking of these tools in my research.
    1. How exactly we can use the useMemo hook.
    1. What are more built-in hooks that I haven't heard about yet and when are the times that I will lean towards using them.
1. What are you most excited about trying to implement or see how it works?
    - useMemo. Memoization is important in reducing redundancy and optimizing storage and I am excitied to see how it can be implemented.

### Preparation Materials

- [context api](https://reactjs.org/docs/context.html)
- [hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
- [react context links](https://github.com/diegohaz/awesome-react-context)
