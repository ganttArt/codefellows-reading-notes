# Readings: Data Modeling

## Review, Research, and Discussion

1. Name 3 advantages to Test Driven Development
    - Easier to refactor
    - High test coverage
    - Less of an inclination to manual test every change you make
    - src: [geeks4geeks](https://www.geeksforgeeks.org/advantages-and-disadvantages-of-test-driven-development-tdd/)
1. In what case would you need to use beforeEach() or afterEach() in a test suite?
    - You need to initialize some data in a database and then remove it when done with the tests.
1. What is one downside of Test Driven Development
    - Tests got to be maintained when requirements change
    - src: [geeks4geeks](https://www.geeksforgeeks.org/advantages-and-disadvantages-of-test-driven-development-tdd/)
1. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
    - Syntax
1. Why REST?
    - REST makes efficient use of bandwidth, as it's much less verbose than SOAP
    - src: [stormpath](https://stormpath.com/blog/rest-vs-soap#:~:text=REST%20also%20makes%20efficient%20use,better%20support%20for%20browser%20clients.)

## Vocabulary Terms

- functional programming - a programming paradigm where programs are constructed by applying and composing functions. It is a declarative programming paradigm in which function definitions are trees of expressions that map values to other values, rather than a sequence of imperative statements which update the running state of the program. src: [wiki](https://en.wikipedia.org/wiki/Functional_programming)
- object-oriented programming (OOP) - a programming paradigm based on the concept of "objects", which can contain data and code: data in the form of fields (often known as attributes or properties), and code, in the form of procedures (often known as methods). src: [wiki](https://en.wikipedia.org/wiki/Object-oriented_programming)
- class - a defined structure to create an object. src: [wiki](https://simple.wikipedia.org/wiki/Class_(programming)#:~:text=A%20class%20is%20written%20by,all%20objects%20of%20one%20type.)
- super - a keyword used to access and call functions on an object's parent. src: [mdn]https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/super)
- this - keyword refers to the object it belongs to. src: [w3schools](https://www.w3schools.com/js/js_this.asp)
- Test Driven Development (TDD) - a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases. src: [wiki](https://en.wikipedia.org/wiki/Test-driven_development#:~:text=Test%2Ddriven%20development%20(TDD),software%20against%20all%20test%20cases.)
- Jest - a JavaScript testing framework designed to ensure correctness of any JavaScript codebase. src: [jest](https://jestjs.io/)
- Continuous Integration (CI) - the practice of merging all developers' working copies to a shared mainline several times a day. src: [wiki](https://en.wikipedia.org/wiki/Continuous_integration)
- REST - a software architectural style which uses a subset of HTTP. Such a Web service must provide its Web resources in a textual representation and allow them to be read and modified with a stateless protocol and a predefined set of operations. src: [wiki](https://en.wikipedia.org/wiki/Representational_state_transfer)
- Data Model - an abstract model that organizes elements of data and standardizes how they relate to one another and to the properties of real-world entities. src: [wiki](https://en.wikipedia.org/wiki/Data_model#:~:text=A%20data%20model%20(or%20datamodel,properties%20of%20real%2Dworld%20entities.)

## Preview

[sql vs nosql video](https://www.youtube.com/watch?v=ZS_kXvOeQ5Y)  
[nosql vs sql](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)  
[nosql modeling techniques](https://highlyscalable.wordpress.com/2012/03/01/nosql-data-modeling-techniques/)  
[mongoose api](https://mongoosejs.com/docs/api.html#Model)  

- Which 3 things had you heard about previously and now have better clarity on?
  - SQL databases are good fit for the complex query intensive environment
  - NoSQL database are highly preferred for large data sets
  - SQL Databases:
    - MySQL
    - MS SQL
    - Oracle
    - SQLite
    - PostgreSQL
  - NoSQL Databases:
    - MongoDB
    - CouchDB
    - Redis
- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - Techniques for scaling MongoDB
  - When to use other NoSQL databases like Redis
  - How to actaully change the structure of the data after there is already data in the db.
- What are you most excited about trying to implement or see how it works?
  - Make a MongoDB with multiple models.
