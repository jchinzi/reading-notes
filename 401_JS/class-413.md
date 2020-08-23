## Bearer Authentication

**Bearer Token** is a secondary authentication method that can be used instead of repeatedly using Basic Authentication or OAuth from the same client

  - Encoded JSON objects that 'bear' enough information for the server to assert that any client request that presents a valid token must have originated from a client that has previously authenticated themselves using either Basic or OAuth

  - Token must be included in the header for all future requests to the server

  ```
  Authorization: Bearer encoded.jsonwebtoken.here
```

Express Server Example:

```
app.get('/somethingsecret', bearerToken, (req,res) => {
  res.status(200).send('secret sauce');
});

function bearerToken( req, res, next ) {
  let token = req.headers.authorization.split(' ').pop();
  try {
    if ( tokenIsValid(token) ) { next(); }
  }
  catch(e) { next("Invalid Token") }
}

function tokenIsValid(token) {
  let parsedToken = jwt.verify(token, SECRETKEY);
  return Users.find(parsedToken.id);
}
```

## JSON Web Tokens
[JWT](https://jwt.io/introduction/)
[What is JWT? (Video)](https://www.youtube.com/watch?v=926mknSW9Lo)

- An open standard that defines a compact and self-contained way for securely transmitting information between parties as a JSON object
  - Compact: can be sent via URL, POST request, HTTP Header
  - Self Contained: Contains information about the user and avoids querying the database more than once

- The Header contains 2 elements:
  - *alg*: Algorithm (ex. HMAC SHA356, RSA)
  - *typ*: Type of JWT token

- The Payload Contains:
  - *claims*: user details or additional metadata

- The Signature combines the base64 Header and the base64 Payload with a secret to provide security

- JWT is digitally signed in one of two ways:
  - Using a secret (with the HMAC algorithm)
  - Using a public/private key pair using RSA or ECDSA

- Signed tokens verify the integrity of the claims contained within
  - This means that you can trust that the contents were not modified & that the generator of the token was trusted
  - This *does Not mean* that the contents are secure - they are viewable and should be treated as such

## When should you use JSON Web Tokens?

- Authorization
  - Allows for 'single sign on' functionality
- Information Exchange
  - The fact that JWT's are signed allows one to confirm the identity of the sender

---

[Home](https://jchinzi.github.io/reading-notes/)