# Reading: Application State with Redux

## Review, Research, and Discussion

1. What are the advantages of storing tokens in “Cookies” vs “Local Storage”
    - Cookies are primarily for reading server-side, local storage can only be read by the client-side. So the question is, in your app, who needs this data — the client or the server? [src](https://stackoverflow.com/questions/3220660/local-storage-vs-cookies)
1. Explain 3rd party cookies.
    - are cookies that are stored under a different domain than you are currently visiting. They are mostly used to track users between websites and display more relevant ads between websites. [src](https://cookie-script.com/all-you-need-to-know-about-third-party-cookies.html)
1. How do pixel tags work?
    - You add the tracking pixel using a code in your site’s HTML code or email, which contains an external link to the pixel server. When someone visits your website, the HTML code is processed by their browser, which follows the link and opens the hidden graphic. This action is identified and recorded in the server’s log files. This method allows for different information about the visitor to be transmitted. [src](https://whatagraph.com/blog/articles/tracking-pixel)

## Document the following Vocabulary Terms

- **cookies** - text files with small pieces of data — like a username and password — that are used to identify your computer as you use a computer network. ... Data stored in a cookie is created by the server upon your connection. [src](https://www.kaspersky.com/resource-center/definitions/cookies#:~:text=Cookies%20are%20text%20files%20with,you%20use%20a%20computer%20network.&text=Data%20stored%20in%20a%20cookie,the%20server%20upon%20your%20connection.)
- **authorization** - Authorization is a security mechanism used to determine user/client privileges or access levels related to system resources, including computer programs, files, services, data and application features. Authorization is normally preceded by authentication for user identity verification. [src](https://www.techopedia.com/definition/10237/authorization#:~:text=Authorization%20is%20a%20security%20mechanism,authentication%20for%20user%20identity%20verification.)
- **access control** -  the selective restriction of access to a place or other resource while access management describes the process. [src](https://en.wikipedia.org/wiki/Access_control)
- **conditional rendering** - In React, you can create distinct components that encapsulate behavior you need. Then, you can render only some of them, depending on the state of your application. [src](https://reactjs.org/docs/conditional-rendering.html)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    1. Redux holds all of the states for your application in one place.
    1. The reducer is a pure function that evaluates the type of action and creates a new state.
    1. Action, Reducer, Store. These are the 3 steps that you use to update state using redux.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    1. Separating the actions and reducers into separate directories/files.
    1. Diving deeper into Redux DevTools chrome extension.
    1. How do we use a Thunk in Redux, what the heck is it?
1. What are you most excited about trying to implement or see how it works?
    - Using Redux in a larger project and seeing how well it can scale up.

### Preparation Materials

- [Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux)

### Bookmark

- [worlds easiest guide to redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)
- [testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)
- [Redux Docs](https://redux.js.org/)
