# Readings: Express REST API

## Review, Research, and Discussion

1. Name 3 real world use cases where you’d want to change the request with custom middleware
    - Parse/clean up the body of a request
    - Check user authentication and throw error if not authenticated
    - Add some extra key/value pairs to the request object based on the data you received
1. True or false: The route handler is middleware?
    - False: route handlers normally do not contain a next, which would make it middleware
1. In what ways can a middleware function end the process and send data to the browser?
    - It can throw an error if the request does not contain what it needs. Or you can just do a send instead of a next in the middleware.
1. At what point in the request lifecycle can you “inject” middleware?
    - Right after the server receives the request and hits the endpoint.
1. What can cause express to error with “Request headers sent twice, cannot start a second response”
    - Calling res.writeHead to early
    - Calling res.redirect then setting more data
    - Calling next after response has been returned
    - from [https://www.endyourif.com/cant-set-headers-after-they-are-sent/](https://www.endyourif.com/cant-set-headers-after-they-are-sent/)

## Vocabulary Terms

- Middleware - software that acts as a bridge between an operating system or database and applications, especially on a network. src: google dictionary
- Request Object - The request object allows you to submit a POST or GET request to an URL. Essentially it provides a way to make REST API requests to another URL. src: [branchcms](https://www.branchcms.com/learn/docs/developer/twig/request-object)
- Response Object - It is the object which communicates between the server and the output which is sent to the client. src: [4guysfromrolla](https://www.4guysfromrolla.com/webtech/faq/Beginner/faq3.shtml)
- Application Middleware - Middleware in the context of distributed applications is software that provides services beyond those provided by the operating system to enable the various components of a distributed system to communicate and manage data.  src: [wiki](https://en.wikipedia.org/wiki/Middleware_(distributed_applications))
- Routing Middleware - Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router(). src: [express docs](https://expressjs.com/en/guide/using-middleware.html#middleware.router)
- Test Driven Development - software development process relying on software requirements being converted to test cases before software is fully developed. src: [wiki](https://en.wikipedia.org/wiki/Test-driven_development)
- Behavioral Testing - Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing. src: [tutorialspoint](https://www.tutorialspoint.com/software_testing_dictionary/behaviour_testing.htm#:~:text=Behavioural%20Testing%20is%20a%20testing,is%20usually%20a%20functional%20testing.)

## Preview

[Review: ES6 Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
[Using Express Routing](https://expressjs.com/en/guide/routing.html)
[Express Routing](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4)

- Which 3 things had you heard about previously and now have better clarity on?
  - ES6 Classes, we used these in 201 and now I just know that these are referred to as ES6 classes as opposed to anything else.
  - res.send() vs. res.json() - can send various things in a send, only a json in res.json
  - How using a method in a class compares to using .prototype methods in constructors.
- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - Using express.Router()
  - Using mixins in ES6 classes
  - What to do in the case when the tool you're using is not compatible with a browser, for instance ES6 classes not being compatible with IE.
- What are you most excited about trying to implement or see how it works?
  - Implementing the express router
