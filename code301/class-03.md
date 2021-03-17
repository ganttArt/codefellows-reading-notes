# Class 3: Passing Functions as Props

## [Lifting Up State](https://reactjs.org/docs/lifting-state-up.html)

- Lifting the state shared by several components up to their closest common ancestor
- Creating Temperature calculator that tells if an input temp is hot enough to boil water
- Input can be in Celsius or Fahrenheit. Stored in scale prop as either “c” or “f” of TemperatureInput component
- c and f inputs have to be synced, via conversion functions toCelsius() and toFahrenheit()
  - The state shared between those 2 TemperatureInput components is lifted up to their closest common ancestor : Calculator component
  - Make the component “controlled” , aka it can have a value and an OnChange event
- Only storing the latest input value and scale is enough, the value on the other scale can be inferred.
- Instead of trying to sync the state between different components, you should rely on the [top-down data flow](https://reactjs.org/docs/state-and-lifecycle.html#the-data-flows-down) -> for less work to find and isolate bugs

## [Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)

- loop through the numbers array using the JavaScript [map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map) function. We return a `<li>` element for each item. Finally, we assign the resulting array of elements to listItems
- A “key” is a special string attribute you need to include when creating lists of elements. They help React identify which items have changed, are added, or are removed. Best way to pick a key is to use a string that uniquely identifies a list item, like id.
- If you choose not to assign an explicit key to list items then React will default to using indexes as keys.
- A good rule of thumb is that elements inside the map() call need keys.
- Keys only need to be unique among siblings.

## [React Tutorial continued through Declaring A Winner](https://reactjs.org/tutorial/tutorial.html)

- Shared state of Square components is lifted to Board
- Board modified to instruct each individual Square about its current value ('X', 'O', or null).
- When a square is clicked, it will let the board know.
  - We’re passing down two props from Board to Square: value and onClick. The onClick prop is a function that Square can call when clicked.
- Square components no longer maintain state, they receive values from the Board component and inform the Board component when they’re clicked. In React terms, the Square components are now controlled components. The Board has full control over them.
- 2 approaches to changing data-mutating the values or replace the data with a new copy
- Immutability
  - makes complex features like “time travel” easier where you can jump back to previous states of the board.
  - makes it easier to detect changes.
  - Helps you build pure components in React. If something has changed then component requires re-rendering.
- change the Square to be a function component.
- Build Taking turns functionality:
  - set the first move to be “X” by default.
  - Each time a player moves, xIsNext (a boolean) will be flipped to determine which player goes next and the game’s state will be saved.
- calculateWinner()
- Timetravel:
  - Lift history state from Board to Game component
  - update the Game component’s render function to use the most recent history entry

## [The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

- spread operator is ... three dots
- "When ...arr is used in the function call, it ‘expands’ an iterable object arr into the list of arguments." — JavaScript.info
- Passing just an array in here wouldn't work: `Math.max(...[1,3,5])`
- This syntax spreads the list into separate arguments
- Works for a string too
- Can be used to make a copy of an array
- Can be used to concatenate arrays (combine them)
- Can be used to add items to start or end of a list
- Can be used to combine objects
- Can be used to create a list of DOM nodes
- Doesn't work on older browsers
- Using the spread operator creates a new reference, always copying them.
- Doesn't work with nested arrays
