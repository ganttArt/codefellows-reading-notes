# Class 9 - Functional Programming

## [Concepts of Functional Programming in Javascript](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

- Immutability and pure functions are functional programming concepts.
- Functional programming avoids changing state and mutating data
- What makes a function pure?
  - It returns the same result if given the same arguments.
  - Doesn’t rely on external objects like global constants
  - Doesn’t read external files
  - Doesn’t contain random number generation
  - Does not cause any side effects like changing the value of a global object, or a param passed by reference.
  - Pure functions are stable, consistent and predictable.
- Benefits of pure functions is they are easier to test because mocking not required.
- Immutability
  - When data is immutable, its state can’t be changed after it’s created.
  - Mutability in interaction can be handled by using recursion.
- Referential transparency aka a function consistently yields the same result for the same input
- Functions as first-class entities aka  they can be treated as values and passed like data. E.g:

```javascript
const sum = (a, b) => a + b;
const subtraction = (a, b) => a - b;

const doubleOperator = (f, a, b) => f(a, b)*2

doubleOperator(sum, 3, 1); //8
doubleOperator(subtraction, 3, 1); //4
```

- Higher-order functions are those that take one or more functions as arguments, OR return a function as their result.
- Map transforms a collection by applying a function to all its elements and building a new collection from its returned values
- Ides of Reduce is to receive a function and a collection and return a value by combining the items

## [Refactoring JavaScript for Performance and Readability](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

There's a middle ground between speed and comprehension and that's where good code lives.

### Scenario 1: Url shortening website

- Refactor the data-structure of URLstore to a map instead of an array for faster lookups on avg.

### Scenario 2: Generate random urls with friendly-words instead of gibberish

- Break up createUser() for readability
- Separate common logic into its own function

### Strategies for writing readable code:

- Return early from functions
- Cache variables and give them good names
- Check for existing Web APIs before writing your own functionality
