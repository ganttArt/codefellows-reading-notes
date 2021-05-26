# Readings: Component Composition

## Review, Research, and Discussion

1. Can a parent component access the state of a child component?
    - Only if there is a method that is being passed down through props that will pass the state back up to the parent. But that is a work around for React's one way data flow.
1. What can be passed along in a prop variable?
    - data stored in a variable or a function
1. How can a child component “know” the state of another component?
    - if that state is passed into the component as props.

## Document the following Vocabulary Terms

- **component props** - “Props” is a special keyword in React, which stands for properties and is being used for passing data from one component to another. But the important part here is that data with props are being passed in a uni-directional flow. ( one way from parent to child) [src](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwit4Kmq4OfwAhVkDzQIHRCEBc0QFjAFegQIBRAD&url=https%3A%2F%2Fitnext.io%2Fwhat-is-props-and-how-to-use-it-in-react-da307f500da0&usg=AOvVaw2094RlAHeiQq7UW8X0bnwd)
- **component state** - The state is an instance of React Component Class can be defined as an object of a set of observable properties that control the behavior of the component. In other words, the State of a component is an object that holds some information that may change over the lifetime of the component. [src](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiv-L_s4OfwAhUpHzQIHcj7BD8QFjACegQIBRAD&url=https%3A%2F%2Fwww.geeksforgeeks.org%2Freactjs-state-react%2F&usg=AOvVaw0MDv3GOvcmeEyTQZRTEp_P)
- **application state** - the state at which an application resides with regards to where in a program is being executed and the memory that is stored for the application. The web is "stateless," meaning everytime you reload a page, no information remains from the previous version of the page. [src](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwivvKGQ4efwAhUDPH0KHZD8CfgQFjABegQIBhAD&url=https%3A%2F%2Fstackoverflow.com%2Fquestions%2F8102674%2Fwhat-is-application-state%2F8102688&usg=AOvVaw17mBGD5-jL-KtFd38Hf1yh)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - That there is a way we can use If->Then statements in react besides ternaries, but you need to import a npm package called react-if to do so.
    - Another approach to building a modal is to use the react-modal npm package. You don't just need to use bootstrap.
    - You can use index.js as the root js file in a subdirectory and react/node will recognize it as the root file of that directory.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Using React-If in a React project
    - Going deeper in to React testing usig rtl's async methods
    - How Redux handles state management. Is it keeping track of component level or application level state?
1. What are you most excited about trying to implement or see how it works?
    - Using functional components

### Preparation Materials

- [react basics recap](https://medium.freecodecamp.org/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030)
- [props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)
- [composition vs inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
- [react testing library api example](https://testing-library.com/docs/react-testing-library/example-intro)

### Bookmark

- [react-if component](https://www.npmjs.com/package/react-if)
- [react-testing-library-async](https://testing-library.com/docs/dom-testing-library/api-async)
