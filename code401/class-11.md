# Readings: Event Driven Applications

## Review, Research, and Discussion

1. Why is access control important?
    - Because you don't want any given user being able to access all of the sensitive information that can be stored in a web application. You may also want some people to have the ability to see and update this more sensitive information.
1. Describe an application that would need access control.
    - Literally anything that has users. Consider Facebook, the users have the ability to make posts, comment on other posts etc., but they wouldn't be able to view a user they aren't friends with. Hypothetically, an admin at facebook, consider that Zuckerberg would probably be able to see any user they wanted to, to see every action they've ever made and sites that the users have been to after Facebook attaches '3rd party cookies'.
1. What is a role used for?
    - To define how much access a user will have.
1. Why is role based access control more scalable than discretionary or mandatory access control?
    - Because if you want to change the access for a large set of people, you only need to change one line of code, instead of having to go through a data base and change permissions for thousands of users.

## Vocabulary Terms

- Authorization - Authorization is the function of specifying access rights/privileges to resources, which is related to general information security and computer security, and to access control in particular. More formally, "to authorize" is to define an access policy. [src](https://en.wikipedia.org/wiki/Authorization)
- Role Based Access Control - an approach to restricting system access to authorized users. It is used by the majority of enterprises with more than 500 employees, and can implement mandatory access control or discretionary access control. [src](https://en.wikipedia.org/wiki/Role-based_access_control)
- Capabilities - (known in some systems as a key) is a communicable, unforgeable token of authority. It refers to a value that references an object along with an associated set of access rights. A user program on a capability-based operating system must use a capability to access an object. [src](https://en.wikipedia.org/wiki/Capability-based_security#:~:text=A%20capability%20(known%20in%20some,capability%20to%20access%20an%20object.)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - How there are so many more methods that you can call on an event beyond event.preventDefault(). Event-driven programming is a whole thing.
    - Clicks and keydowns trigger events, lots of this stuff is taken care of for us in frameworks like React, where we use an on change.
    - An Event-driven programming use case could be for building a game, where every click and keyclick needs to be heard immediately and triggers something.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Examples of using event-driven programming for our purposes.
    - How to use socket.io and it's primary use cases.
    - More about TCP, how this differs from HTTP and when we use one or the other.
1. What are you most excited about trying to implement or see how it works?
    -  Using EventEmitter

## Preparation Materials

- [Event Driven Programming](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming)
- [Node docs: events](https://nodejs.org/api/events.html)
