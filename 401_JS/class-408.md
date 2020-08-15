Routes can be managed in separate modules from the main server, allowing us to extract that logic and wiring to be more topical.

How does this change the server’s role?

index.js - Entry Point
server.js - Hub, Exported Server
models/categories.js, etc - Data Models
routes/categories.js, etc - Routers and Handlers

---

[Home](https://jchinzi.github.io/reading-notes/)