## User Modeling

* There are many situations where users may submit sensitive data to a site for storage:
  - Personal: Email Address, Home Address, Name, etc.
    - This type of data is generally considered 'safe enough' behind a firewall and/or within a password protected database
  - Secret: Passwords, SSN, etc.
    - This type of data (that shouldn't be available to anyone, including devs with permissions) should be encrypted before storage using a hashing algorithm
* In applications that allow users to access others 'personal' information, it is then considered best practice create secondary profile models to hold only that data that should be shared and limit user access to that secondary model

## Cryptography

**Cryptography**: The science which studies methods for encoding messages so that they can be read only by a person with the information necessary (known as the *key*) to decrypt them

**Cryptanalysis**: The science of decoding encrypted messages without the proper *key*

## Hash Algorithms

* Algorithms that take in data and return a consistent but difficult to reverse hash
  - This is useful because:
    - The hashed version of sensitive information (like a password) can safely be stored with less fear of malicious use if accessed
    - The same initial data passed into the algorithm will produce the same hash, so a user reentering their password will be validated by comparing the hash of their provided password with the hash on file that was generated from the 'correct' password

## Cypher Algorithms

* Algorithms that take in data and a key to return encrypted data.  That data can later be decrypted by using the same key
  - This is accomplished by creating user tokens (made by associating a random unique string called a a tokenSeed with a user account)
    - The tokenSeed is then encrypted with a secret key known only to the server
    - When future requests are made by the user, they send their user token and the server is able to use the tokenSeed to decrypt the token and match that user to the corresponding database entry

## Basic Authorization

* Method used to send a username and password in an HTTP request
  - This method uses base64 encoding and sets the resulting value as an Authorization header that can be decoded by the server
  - Once the server decodes the username and password that information can be checked for validation
  - If the combo is validated, the server will respond to the client with a validation response (token or key) so that in the future the user can re-authenticate without performing basic authorization again.
  - This is **not** a form of encryption

Browser Example:
```
let encoded = window.btoa('someusername:P@55w0rD!')
// c29tZXVzZXJuYW1lOlBANTV3MHJEIQ==

let decoded = window.atob('c29tZXVzZXJuYW1lOlBANTV3MHJEIQ==');
// someusername:P@55w0rD!

request({
  method: 'GET',
  url: 'https://api.example.com/login',
  headers: {
    Authorization: `Basic ${encoded}`,
  },
})
.then(handleLogin)
.catch(handleLoginError)
```

Node Example:
```
let base64 = require('base-64');

let string = 'someusername:P@55w0rD!';
let encoded = base64.encode(string); // c29tZXVzZXJuYW1lOlBANTV3MHJEIQ==
let decoded = base64.decode(encoded); // someusername:P@55w0rD!
```
---

[Home](https://jchinzi.github.io/reading-notes/)