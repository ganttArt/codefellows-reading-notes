# Readings: Message Queues

## Review, Research, and Discussion

1. What does it mean that web sockets are bidirectional? Why is this useful?
    - It means that clients can send information to the sever and vice versa. This is useful because it allows an exchange of information and for the sockets to conform to the Transmission Control Protocol.
1. Does socket.io use HTTP?
    - The client will try to establish a WebSocket connection if possible, and will fall back on HTTP long polling if not. [src](https://socket.io/docs/v4/index.html)
1. What happens when a client emits an event?
    - It is sent to the server, and the server will handle that by listening for it.
1. What happens when a server emits an event?
    - It is sent out to a specific client or to all clients.
1. What happens if a client “misses” an event? How can we mitigate this?
    - That shouldn't be too much of a problem because you are relying on TCP which should make it so the client has to confirm that they've received the data packets. We could implement some error handling on the server side if there is an issue.

## Document the following Vocabulary Terms

- **Socket** - When a computer program needs to connect to a local or wide area network such as the Internet, it uses a software component called a socket. The socket opens the network connection for the program, allowing data to be read and written over the network. [src](https://techterms.com/definition/socket#:~:text=When%20a%20computer%20program%20needs,and%20written%20over%20the%20network.)
- **Web Socket** - a computer communications protocol, providing full-duplex communication channels over a single TCP connection. [src](https://en.wikipedia.org/wiki/WebSocket)
- **Socket.io** - Socket.IO enables real-time, bidirectional and event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. [src](https://socket.io/)
- **Client** - In computing, a client is a piece of computer hardware or software that accesses a service made available by a server as part of the client–server model of computer networks. The server is often (but not always) on another computer system, in which case the client accesses the service by way of a network. [src](https://en.wikipedia.org/wiki/Client_(computing)#:~:text=In%20computing%2C%20a%20client%20is,by%20way%20of%20a%20network.)
- **Server** - A server is a computer that provides data to other computers. It may serve data to systems on a local area network (LAN) or a wide area network (WAN) over the Internet. [src](https://techterms.com/definition/server#:~:text=A%20server%20is%20a%20computer,(WAN)%20over%20the%20Internet.&text=For%20example%2C%20a%20computer%20connected,%2C%20print%20server%2C%20or%20both.)
- **OSI Model** - (Open Systems Interconnection Model) is a conceptual framework used to describe the functions of a networking system. The OSI model characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software. [src](https://www.forcepoint.com/cyber-edu/osi-model#:~:text=The%20OSI%20Model%20(Open%20Systems,between%20different%20products%20and%20software.)
- **TCP/IP Model** - a concise version of the OSI model. It contains four layers, unlike seven layers in the OSI model. The layers are: Process/Application Layer, Host-to-Host/Transport Layer, Internet Layer, Network Access/Link Layer. [src](https://www.geeksforgeeks.org/tcp-ip-model/)
- **TCP** - (Transmission Control Protocol) is a standard that defines how to establish and maintain a network conversation through which application programs can exchange data. TCP works with the Internet Protocol (IP), which defines how computers send packets of data to each other. [src](https://searchnetworking.techtarget.com/definition/TCP#:~:text=TCP%20(Transmission%20Control%20Protocol)%20is,of%20data%20to%20each%20other.)
- **UDP** - (User Datagram Protocol) is a communications protocol that is primarily used for establishing low-latency and loss-tolerating connections between applications on the internet. It speeds up transmissions by enabling the transfer of data before an agreement is provided by the receiving party. [src](https://searchnetworking.techtarget.com/definition/UDP-User-Datagram-Protocol#:~:text=UDP%20(User%20Datagram%20Protocol)%20is,provided%20by%20the%20receiving%20party.)
- **Packets** - a small segment of a larger message. Data sent over computer networks, such as the Internet, is divided into packets. These packets are then recombined by the computer or device that receives them. [src](https://www.cloudflare.com/learning/network-layer/what-is-a-packet/#:~:text=In%20networking%2C%20a%20packet%20is,or%20device%20that%20receives%20them.)

## Preview

1. Which 3 things had you heard about previously and now have better clarity on?
    - That socket.io can be integrated with Express.js. On hitting an endpoint, a socket can listen for that and do something.
    - Implementing a chat server would look as simple as emiting messages, when these messages are connected to the url... not to simple but understandable in a bigger picture.
    - You can emit to several rooms at the same time.
1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
    - Integrating socket.io with a restful api.
    - Connecting socket.io events to endpoints on the front end.
    - How to mitigate the circumstance when the client misses an event.
1. What are you most excited about trying to implement or see how it works?
    - Integrating socket.io with an express server.

## Preparation Materials

[Socket.io Chat Example](https://socket.io/get-started/chat/)
[Rooms and Namespaces](https://socket.io/docs/rooms-and-namespaces/)
[Socket.io Emit Cheatsheet](https://socket.io/docs/emit-cheatsheet/)