# Readings: Authentication

## Review, Research, and Discussion

1. Explain what a “Singleton” is (in Computer Science terms)
    - An object that can only be instantiated once.
1. Explain how the Singleton pattern can be used with Node modules, specifically with classes
    - Create two classes. One that you can use to create a singleton, the other to check if it has already been instantiated. Checkout how to do it [here](https://medium.com/swlh/node-js-and-singleton-pattern-7b08d11c726a).
1. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
    - When I construct it I need a (req, res, next). When I do what I need to do with the middle ware i will call next(). To use it, when I create the route I will call the middleware between the endpoint and (req, res).

## Vocabulary Terms

- Router Middleware
  - Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router(). src [express](https://expressjs.com/en/guide/using-middleware.html#middleware.router)
- Dynamic Module Loading
  - a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory. src: [wiki](https://en.wikipedia.org/wiki/Dynamic_loading)
- Singleton Pattern
  - the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. src: [wiki](https://en.wikipedia.org/wiki/Singleton_pattern)
- CRUD -> REST Method Matches
  - Create -> POST
  - Read -> GET
  - Update -> PUT/PATCH
  - Delete -> DELETE
- Mock Testing
  - Mock testing is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. src: [devopedia](https://devopedia.org/mock-testing#:~:text=Mock%20testing%20is%20an%20approach,behaviour%20of%20the%20real%20ones.)

## Preview

- [Securing Passwords](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html)
- [Basic Auth](https://en.wikipedia.org/wiki/Basic_access_authentication)
- [OWASP auth cheatsheet](https://www.owasp.org/index.php/Authentication_Cheat_Sheet)
- [bcrypt docs](https://www.npmjs.com/package/bcrypt)

1. Which 3 things had you heard about previously and now have better clarity on?
    - bcrypt works well because it uses a technique called Key Stretching
    - The authorization pattern where username and password are combined with a single colon (:), is in line with the standard for basic access authentication for a HTTP transaction. src: Reading 2
    - Why to use async with bcrypt: "If you are using bcrypt on a simple script, using the sync mode is perfectly fine. However, if you are using bcrypt on a server, the async mode is recommended. This is because the hashing done by bcrypt is CPU intensive, so the sync version will block the event loop and prevent your application from servicing any other inbound requests or events. The async version uses a thread pool which does not block the main event loop." src: Reading 4
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - What's the deal with hashing? How does it relate to a hashmap/dictionary?
    - Why is username:password a pattern we use and when are we actually passing that in?
    - How to handle "Forgot password" case.
1. What are you most excited about trying to implement or see how it works?
    - Setting different permissions for different users.
