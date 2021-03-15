# Introduction to React and Components

## [Passing Data Through Props](https://reactjs.org/tutorial/tutorial.html)

- A component takes in parameters called props, and returns a hierarchy of views to display via the render method
- use React.createElement to create a new tag element
- Each react element is a javascript object, javascript goes in braces in JSX
- Refer to components using a tag with the components name `<ShoppingList />`
- Pass a prop into a parent components render method and then call that value in the child component by using `this.props.value`

## [React Hello World](https://reactjs.org/docs/hello-world.html)

The smallest React example contains these elements

``` javascript
ReactDOM.render(
  <h1>Hello, World!</h1>
  document.getElementById('root')
);
```

## [Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)

- JSX is like template language but with JavaScript in it, it is a syntax extension to JavaScript
- Separates concerns (components), not separating the business logic and the presentation. Basically, no separation of HTML and JavaScript
- Insert javascript variable into a html taged element by using curly braces
- Can store html as a js variable
- Can do everything with jsx that you can do with javascript objects, such as using conditionals and loops. Because after compiliation jsx evaluates to js objects
- Attributes for html tags can be included by using curly braces or string literals to define the attibutes
- React DOM uses camelCase property naming convention instead of html attribute names
- It is safe to embed user input in JSX because there is inbuilt protection against injection attacks.
- Use Babel language definition in code editor for syntax highlighting

## [Rendering Element](https://reactjs.org/docs/rendering-elements.html)

- use `ReactDOM.render(element, document.getElementById('root'))` to render
- React elements are immutable, to update the UI you must create a new element and pass it to the ReactDOM.render method.
- React only updates what's necessary, by comparing the previous element and the new element.
  - Even though we include a whole UI tree, only the part that's content changes will get updated

## [Components and Props](https://reactjs.org/docs/components-and-props.html)

- You can write components using functions or classes. It will take that shape and return a React element.

``` javascript
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}

class Welcome extends React.Component {
  render() {
    return <h1>Hello, {this.props.name}</h1>;
  }
}
```

- Props will be passed in when you call the user defined component like in this format `<Welcome name="Sara" />`
- Always start component name with a capital letter
- Break down the components as small as they make sense and are useable
- name props from the components own point of view, not based on the context which it is being used this time becuase that may change in the future.
- Components in components in components etc.
- If a part of your UI is used several times, or is complex enough on it's own, it is a good candidate to be extracted to a separate component
- Within a function you cannot modify a prop. Props are read only. Do not change the inputs of a function, and in this case, do not modify the props you've had passed in.

[<== Back](../README.md)
