### September 2<sup>nd</sup>
## Message Queues

1. What does it mean that web sockets are bidirectional? Why is this useful?
- Web sockets are bidirectional because you can push information both ways, from client to server and from server to client.

2. Does socket.io use HTTP? Why?
- Socket.io does use HTTP to make the initial connection even when websockets can be used

3. What happens when a client emits an event?
- When a client emits an event, the server is listening for it and then handles it however it has been told to.

4. What happens when a server emits an event?
- When a server emits an event, it is emitted to wherever it's been told. It goes back to a client that's listneing for it, accepts the payload and then goes on with its business.

5. What happens if a client “misses” an event?
- There isn't any error handling when using sockets.io, so it's a best-efforts process. Unhandled events are just ignored.

6. How can we mitigate this?
- We can use a queue! We can keep the messages in a structure (maybe just an object) that we treat as a queue and each time one is received we'll delete it from the queue, but we can also have a listener to get all messages not received while offline. Cool!

## Common Terminology

|    **Term**    | **Definition**  |
| -------------- | ----------- |
| Web Socket | technology that makes it possible to open a two-way interacive communication session between clients and server  |
| Socket.io | real time, bidirectional event-based communication library    |
| Client | Connected and communicating through server    |
| Server | Connection hub in socket.io, enabling communication between itself and clients |


## Resources
- https://stackoverflow.com/questions/37836130/socket-io-why-does-it-need-an-http-server#:~:text=The%20premise%20on%20which%20your,%2C%20which%20it%20isn't.&text=Even%20when%20websockets%20can%20be,%2Fsocket.io.js%20.