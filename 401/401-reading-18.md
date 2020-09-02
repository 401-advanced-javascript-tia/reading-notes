## Sep 1<sup>st</sup>
## Socket.io

1. What is the benefit of transforming data into packets?
- Data can be sent super fast and efficiently, there's no fuss about error handling. It's a "best effort" protocol. 

2. UDP is often referred to as a connectionless protocol. Why is this?
- Doesn't rely on a connection across the internet between computers. With UDP one program can send a bunch of packets to another and thats it.

3. Can a socket server application have multiple socket connections?
- Yes, a socket server listens on a single port, so it can have multiple socket connections that are associated with the same port they're listening on.

4. Can a socket connection application be connected to multiple socket servers?
- Yes the socket connection app could be connected to multiple servers, one socket per server. 

5. Can an application be both a socket server and a socket connection?
- You could do this with a single application, but they'd have to be using different ports (or at least not the same port at the same time).



## Common Terminology

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| OSI Model |Connectionless internet protocol with multiple messages being sent as packets         |
| TCP Model | Connection-oriented, with established connection data can be sent bidirectional      |
| TCP | Transmission Control Protocol   |
| UDP | User Datagram Protocol    |
| Packets | Small amount of data sent over a network, has a source and destination and content   |
| Socket | A connection to a server. One of the endpoints of the two-way connection link between two programs running on a network   |



## Resources
- https://www.diffen.com/difference/TCP_vs_UDP#:~:text=There%20are%20two%20types%20of,a%20simpler%2C%20connectionless%20Internet%20protocol
- https://techterms.com/definition/packet#:~:text=A%20packet%20is%20a%20small,(or%20data)%20being%20transferred.
