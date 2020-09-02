### Questions:

**What is the benefit of transforming data into packets?**

By transforming data into packets, the data can be sent to its destination by the best available route.  This means that not all packets have to be sent along the same route (which may not be equally efficient for all packets).  After transmission, the packets an be reassembled into the the complete data that they began as.

*Source: https://computer.howstuffworks.com/question525.htm*

**UDP is often refereed to as a connectionless protocol. Why is this?**

A connection requires a 'handshake' in which the receiver agrees to the communication before data is sent.  Because UDP sends data without confirmation, it can be considered a connectionless protocol

*Source: https://www.cloudflare.com/learning/ddos/glossary/user-datagram-protocol-udp/*

**Can a socket server application have multiple socket connections?**

Yes, socket server applications can accommodate many socket connections at once.

**Can a socket connection application be connected to multiple socket servers?**

A client application can connect to multiple socket servers, but each individual socket client can only connect to one server at a time.   Therefore, the client application would need to have multiple client sockets in order to connect with multiple socket servers simultaneously

**Can an application be both a socket server and a socket connection?**

To the best of my understanding, an application can run both client and server sockets - however, the same socket cannot perform both tasks simultaneously

---

### Definitions

|Term|Definition|Source|
|:--|:-:|--:|
|OSI Model|Open Systems Interconnection Model - a conceptual model created by the International Organization for Standardization which enables diverse communication systems to communicate using standard protocols.|https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/|
|TCP Model|TCP/IP Model is used for establishing a connection and communicating through the network|https://techdifferences.com/difference-between-tcp-ip-and-osi-model.html|
|TCP|Transmission Control Protocol - a fundamental protocol within the Internet protocol suite that creates and maintains connections between hosts.|https://techterms.com/definition/tcp|
|UDP|User Datagram Protocol - a communication protocol used across the Internet for especially time-sensitive transmissions such as video playback or DNS lookups.  It speeds up communications by not requiring a 'handshake' (quicker, but open to exploitation)|https://www.cloudflare.com/learning/ddos/glossary/user-datagram-protocol-udp/|
|Packets|Made up of a *header* (containing instructions about the data, such as the length of the packet, synchronization, packet #, protocol, destination address & originating address), a *payload* (the body or data of the packet - may be padded with blank information if the packet is fixed-length), and a *trailer* (also called the footer - typically contains a note indicating that it is the end of the packet)|https://computer.howstuffworks.com/question525.htm|
|Socket|One endpoint of a two-way communication link between two programs running on the network.  A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to|https://docs.oracle.com/javase/tutorial/networking/sockets/definition.html|

---

[Home](https://jchinzi.github.io/reading-notes/)