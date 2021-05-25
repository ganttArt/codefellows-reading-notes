# Reading: Props and State

## Review, Research, and Discussion

1. Does a deployed React application require a server?
    - You don’t necessarily need a static server in order to run a Create React App project in production. It also works well when integrated into an existing server side app.[src](https://create-react-app.dev/docs/deployment/#:~:text=You%20don't%20necessarily%20need,an%20existing%20server%20side%20app.)
1. Why do we prefer to test a React application at the behavior rather than the unit level?
    - Because it is a front end application. You can definitely test some of the business logic happening, but more importantly you want to test how users are going to be using the website by using behavioral tests.
1. What does `npm run build` do?
    - Is used particularly when you want to run a production build as opposed to a development build locally. It doesn't include some of the files that you do not need in a deployment.
1. Describe the actual composition / architecture of a React application
    - At it's simplest you need a package.json, node_modules, index.js and index.html
      - index.html is the setup for the html of the site and contains the root div
      - index.js is the base component which all the other components will live in and connects the components to our base html.

## Document the following Vocabulary Terms

- **BDD** - BDD is a process designed to aid the management and the delivery of software development projects by improving communication between engineers and business professionals. In so doing, BDD ensures all development projects remain focused on delivering what the business actually needs while meeting all requirements of the user. [src](https://inviqa.com/blog/bdd-guide#what-is-it)
- **Acceptance Tests** - a method of software testing where a system is tested for acceptability. The major aim of this test is to evaluate the compliance of the system with the business requirements and assess whether it is acceptable for delivery or not. [src](https://www.geeksforgeeks.org/acceptance-testing-software-testing/)
- **mounting** - Mounting is the phase in which our React component mounts on the DOM (i.e., is created and inserted into the DOM). This method is called just before a component mounts on the DOM or the render method is called. After this method, the component gets mounted. [src](https://www.freecodecamp.org/news/how-to-understand-a-components-lifecycle-methods-in-reactjs-e1a609840630/#:~:text=Mounting%20is%20the%20phase%20in,and%20inserted%20into%20the%20DOM).&text=This%20method%20is%20called%20just,method%2C%20the%20component%20gets%20mounted.)
- **build** -

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - Another approach to creating a react app can be to just install the necessary react packages. `npm i react react-scripts react-dom`
    - State is immutable in React. setState actually creates a copy of state with the change made.
    - BDD is more than just writing user tests, it is a whole design paridigm that focuses on meeting the user needs and also improving communication in the development process.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Writing Behavioral/user tests for React apps.
    - Setting up ci/cd using github actions for React apps.
    - What Redux is, how do we use it, and why would we use it.
1. What are you most excited about trying to implement or see how it works?
    -Writing Behavioral/user tests for React apps.

### Preparation Materials

- [setState explained](https://css-tricks.com/understanding-react-setstate/)
- [handling events](https://facebook.github.io/react/docs/handling-events.html)
- [forms](https://facebook.github.io/react/docs/forms.html)
- [state and lifecycle](https://facebook.github.io/react/docs/state-and-lifecycle.html)
- [components and props](https://facebook.github.io/react/docs/components-and-props.html)
- [React Testing Library](https://testing-library.com/docs/react-testing-library)
- [RTL Testing Example](https://thomlom.dev/beginner-guide-testing-react-apps/)

### Bookmark

- [Roles Reference](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Techniques#Roles)
