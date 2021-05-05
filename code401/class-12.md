# Readings: Socket.io

## Review, Research, and Discussion

1. What is the benefit of transforming data into packets?
    - Packets are intended to transfer data reliably and efficiently. Instead of transferring a large file as a single block of data, sending smaller packets helps ensure each section is transmitted successfully. If a packet is not received or is "dropped," only the dropped packet needs to be resent. [src](https://techterms.com/definition/packet)
1. UDP is often refereed to as a connectionless protocol. Why is this?
    - Because it does not need a response back from the receiving party. This makes sending information faster and is used when the receiver does not necessarily need every bit of information every second. Cases where this is used is streaming video or for video games, but would not be used where data integrity is important like the WWW or emails. (Knowledge gained from video 1 below.)
1. Can a socket server application have multiple socket connections?
    - Yes, you can create a server socket that can handle multiple clients simultaneously. [src](https://www.quora.com/Can-a-socket-of-a-server-be-used-by-multiple-clients-simultaneously)
1. Can a socket connection application be connected to multiple socket servers?
    - Is it possible to bind one process to multiple ports? Yes. Yes, each listening (bound) port is serviced by a separate socket (as are all the connections made from each listening port). [src](https://unix.stackexchange.com/questions/128677/bind-one-process-to-multiple-ports/128679)
1. Can an application be both a socket server and a socket connection?
    - Sure, I think we've even built that already.

## Vocabulary Terms

- Observer Pattern - a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. [src](https://en.wikipedia.org/wiki/Observer_pattern)
- Listener - a procedure or function in a computer program that waits for an event to occur. [src](https://www.computerhope.com/jargon/e/event-listener.htm#:~:text=An%20event%20listener%20is%20a,for%20an%20event%20to%20occur.&text=The%20listener%20is%20programmed%20to,specific%20to%20Java%20and%20JavaScript.)
- Event Handler - a software routine that processes actions such as keystrokes and mouse movements. With Web sites, event handlers make Web content dynamic. [src](https://www.webopedia.com/definitions/event-handler/)
- Event Driven Programming - when a program is designed to respond to user engagement in various forms. It is known as a programming paradigm in which the flow of program execution is determined by “events.” Events are any user interaction, such as a click or key press, in response to prompt from the system. [src](https://www.edgetechacademy.edu/node-js/event-driven-programming/)
- Event Loop - a programming construct or design pattern that waits for and dispatches events or messages in a program. [src](https://en.wikipedia.org/wiki/Event_loop#:~:text=In%20computer%20science%2C%20the%20event,or%20messages%20in%20a%20program.)
- Event Queue - a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system. [src](https://www.techopedia.com/definition/24963/event-queue#:~:text=An%20event%20queue%20is%20a,of%20an%20enterprise%20messaging%20system.)
- Call Stack - a stack data structure that stores information about the active subroutines of a computer program. [src](https://en.wikipedia.org/wiki/Call_stack)
- Emit/Raise/Trigger - To start a process of one kind or another.
- Subscribe - Publish/subscribe messaging, or pub/sub messaging, is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic. [src](https://aws.amazon.com/pub-sub-messaging/)
- database - an organized collection of structured information, or data, typically stored electronically in a computer system. [src](https://www.oracle.com/database/what-is-database/)


## Preview

- Which 3 things had you heard about previously and now have better clarity on?
  - The OSI model was put in place so different operating systems could talk to each other in a standardized way.
  - Sockets are ways to listen for updates from other systems. Sockets can also be used to send out information. Sockets are not just some behind the scenes of programming, but are actually a viable way to create several software solutions like a chat system.
  - Sockets use TCP to exchange data. We may consider even using UDP someday to build something more graphically oriented.
- Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
  - Using Socket.io rooms, in our case to notify specific vendors of new information.
  - More about observer patterns, how we practically apply something like this in our application development.
  - How using sockets in phase 2 differs from using the event loop in phase 1. Are these utilizing different layers of the OSI? Could we implement phase 1 across multiple servers running?
- What are you most excited about trying to implement or see how it works?
  - Building a chat system or connecting what we've done with sockets to an api or browser in some way.

## Preparation Materials

### Additional Resources

#### Videos

- [OSI Model Explained](https://www.youtube.com/watch?v=vv4y_uOneC0)
- [TCP Handshakes Explained](https://www.youtube.com/watch?v=xMtP5ZB3wSk)

#### Read/Skim

- [Web Sockets](https://en.wikipedia.org/wiki/WebSocket)
- [Socket.io Tutorial](https://www.tutorialspoint.com/socket.io/)
- [Socket.io vs Web Sockets](https://www.educba.com/websocket-vs-socket-io/)

#### Bookmark

- [Socket.io Documentation](https://socket.io/docs/)
- [Socket.io Server API](https://socket.io/docs/server-api)
- [Socket.io Client API](https://socket.io/docs/client-api)
- [Socket Testing Tool](https://amritb.github.io/socketio-client-tool/)
