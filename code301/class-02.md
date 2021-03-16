# Class 2 - State and Props

## [State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)

- State is stored in the constructor as an object with key value pairs
- Refer to it with this.state.key
- Using componentDidMount and componentWillUnmount to manage lifecycle. In the example shown, these methods were called with a function called tick to increment a timer every second.
- To re-assign a value to state, must use setState method.
- If you need to re-assign a state value which is dependent on doing some business logic on state and props, pass in both into the setState method like so

```javascript
this.setState((state, props) => ({
  counter: state.counter + props.increment
}));
```

- State is local to the component. It is not accessed by parent component. Child components can access them only if they are passed down, but the child wouldn't know if the value came from it's parents props or state.

## [Handling Events](https://reactjs.org/docs/handling-events.html)

- React events are named using camelCasing. For example onclick is now onClick.
- Must call preventDefault method if you want to prevent default behavior, like a button reloading the page on click.
- To use event listeners, create a listener function, and define it in the constructor as well to bind it.
- To pass a parameter into an event handler you can use either of these formats:

```javascript
<button onClick={(e) => this.deleteRow(id, e)}>Delete Row</button>
<button onClick={this.deleteRow.bind(this, id)}>Delete Row</button>
```

## [Conditional Rendering](ttps://reactjs.org/docs/conditional-rendering.html)

- Conditionals can be used in jsx the same way they are used in js.
- A potentially shorter way to do this is to use curly braces. `{something && html expression}`. If the something evaluates to true, then the html expression will be rendered.
- Using conditional operator for inline conditionals.
  - `condition ? true : false`
  - `The user is <b>{isLoggedIn ? 'currently' : 'not'}</b> logged in.`
  - This is best for oneliners, any more it gets more confusing to read.
- If you don't want something to render, return null.

## [React Tutorial through Dev Tools](https://reactjs.org/tutorial/tutorial.html)

See notes taken for this section in [class 1 notes](class-01.md)

## [Bootstrap with React](https://react-bootstrap.github.io/)

- React-Bootsrap replaces Bootstrap, focusing styling around React components.
- So start trying to use this when you're working with React

## [Netlify](https://www.netlify.com/)

- Netlify works with your git workflow.
- This is a platform to build, deploy and collaborate on web apps.
- A place for deploying scalable applications, includes CI/CD workflow.
- Focused more on front end development.
- On some level a competitor to Heroku, here is a comparison from [Back4App](https://blog.back4app.com/netlify-vs-heroku/)

![Netlify Heroku Comparison](images/Netlify-Heroku-Comparison.png)

[<== Back](../README.md)
