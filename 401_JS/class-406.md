## HTTP

* HTTP stands for *Hyper Text Transfer Protocol*, a stateless request-response application layer protocol

  - Applications built using HTTP subscribe to the client-server computing model

  - **server**: host designed to provide a service
  - **client**: hosts that make requests to the service

## HTTP Requests

 * The first line of a request contains a **method**, **URL**, and **HTTP version**.  Following lines are request **headers**.

 *Key Terms regarding Methods*:

 **safe**: does not change the state of the server - should only be used for information retrieval

 **idempotent**: identical requests of this type will get identical responses, no matter how many times they are called.  All *safe* methods are also *idempotent*

 **cacheable**: the client is able to cache the response

 |HTTP Method|Request has Body|Response has Body|Safe|Idempotent|Cachable|
 |:--|:-:|:-:|:-:|:-:|:-:|
 |GET|no|yes|yes|yes|yes|
 |HEAD|no|no|yes|yes|yes|
 |POST|yes|yes|no|no|yes|
 |PUT|yes|yes|no|yes|no|
 |DELETE|no|yes|no|yes|no|
 |CONNECT|yes|yes|no|no|no|
 |OPTIONS|optional|yes|yes|yes|no|
 |TRACE|no|yes|yes|yes|no|
 |PATCH|yes|yes|no|no|no|

## HTTP Response

 * The first line of a response contains an **HTTP version**, **status code** and **status message**.  Following lines are request **headers**.

## REST

* Acronym for REpresentational State Transfer - a means by which we can reference, manipulate and transfer state.

|REST Method|CRUD Operation|Function|
|:-:|:-:|:--|
|GET|READ|Retrieve 1+ Records|
|POST|CREATE|Create a New Record|
|PUT|UPDATE|Replace Record with an updated version|
|PATCH|UPDATE|Replace the updated portion of the Record|
|DESTROY|DELETE|Remove a Record|

## [What Is A RESTful API? Explanation of REST & HTTP](https://www.youtube.com/watch?v=Q-BpqyOT3a8)

**API**: Application Program Interface - a contract provided by one piece of software to another (request & response)

Video uses the GitHub API as an example of a RESTful API and demonstrates accessing data from the GitHub API using Postman

---

[Home](https://jchinzi.github.io/reading-notes/)