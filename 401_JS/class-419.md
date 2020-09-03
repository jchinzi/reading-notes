### Questions:

**What does it mean that web sockets are bidirectional? Why is this useful?**

Web sockets allow a single TCP socket connection to be hijacked so that the client-server relationship can relay bi-directional, full-duplex messages instantaneously.  This means that messages can be sent and received in real time and memory use is configurable.

*Source: https://medium.com/@nerdplusdog/websocket-simultaneous-bi-directional-client-server-communication-e7948203054b*

**Does socket.io use HTTP? Why?**

Yes - socket.io is a communication library that uses websockets where appropriate, however initial connection setup is done over HTTP.  HTTP is also useful for some transports, and can serve as a fallback for websockets.

*Source: https://stackoverflow.com/questions/37836130/socket-io-why-does-it-need-an-http-server#:~:text=The%20premise%20on%20which%20your,%2C%20which%20it%20isn't.&text=Even%20when%20websockets%20can%20be,%2Fsocket.io.js%20.*

**What happens when a client emits an event?**

Events emitted by the client are sent to the server to be handled.

**What happens when a server emits an event?**

Events emitted by the server can be sent to all connected clients or to a specified segment of clients by specifying a namespace or room.  Clients who receive the event may have functions in place to handle the event.

**What happens if a client “misses” an event?**

Missed events are analogous to unhandled events - nothing 'happens'.

**How can we mitigate this?**

- Confirm that event handlers are in place to perform necessary actions meant to be triggered by events.
- Include error handlers as a second layer of event handling if things don't work as intended

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|Web Socket|Bidirectional, full-duplex protocol that is used in the same scenario of client-server communication but starts from ws:// or wss://.|https://www.geeksforgeeks.org/what-is-web-socket-and-how-it-is-different-from-the-http/|
|Socket.io|JavaScript library for realtime web applications that enables realtime, bi-directional communication between web client and servers.  Includes a client-side library that runs in the browser and a server-side library for Node.js|https://en.wikipedia.org/wiki/Socket.IO|
|Client|The receiving end of a service or the requestor of a service in a client/server model type of system.|https://www.techopedia.com/definition/437/client|
|Server|A computer that provides data to other computers.|https://techterms.com/definition/server#:~:text=A%20server%20is%20a%20computer,the%20purpose%20of%20the%20server.|

---

[Home](https://jchinzi.github.io/reading-notes/)