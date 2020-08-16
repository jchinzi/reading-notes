Routes can be managed in separate modules from the main server, allowing us to extract that logic and wiring to be more topical.

How does this change the server’s role?  For one thing, this should make our code more DRY and readable.

index.js - Entry Point
server.js - Hub, Exported Server
models/categories.js, etc - Data Models
routes/categories.js, etc - Routers and Handlers

## [Routing](https://expressjs.com/en/guide/routing.html)

* **routing**: how an application's endpoints (URIs) respond to client requests

* Route paths can be strings, string patterns, or regular expressions

|Response Method|Description|
|:--|--:|
|res.download()| Prompt a file to be downloaded|
|res.end()|End the response process|
|res.json()|Send a JSON response|
|res.jsonp()|Send a JSON response with JSONP support|
|res.redirect()|Redirect a request|
|res.render()|Render a view template|
|res.send()|Send a response of various types|
|res.sendFile()|Send a file as an octet stream|
|res.sendStatus()|Set the response status code and send its string representation as the response body|

* **app.route()** can be used to create a chainable route handler for a route path

* **express.Router()** class can be used to create  modular, mountable route handlers

---

[Home](https://jchinzi.github.io/reading-notes/)