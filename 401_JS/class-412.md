## OAUTH2.0

**OAuth**: 'an open standard for access delegation 
  - serves as a way to give users the ability to grant application access to services without supplying their password
    - *Auth* refers to Authorization, specifically between services

## How does OAuth work?

1.  Application requests specific permissions from user
1.  User agrees to the above request
1.  Remote service contacts application with one-time-use *Code*
1.  Application calls back to a special address on the remote service to exchange the *Code* for a *Token*
1.  Once the *Token* is granted, the application is able to contact hte remote service using the *Token* to access information on behalf of the user

At this point, the *Token* is for all intents and purposes the User

## Access Code

Clients must grant permission to the application.

* Necessary information is passed through a query string by an `<a>` tag to the authorization server

The request often includes

- `response_type=code` (request for an authorization code)
- `client_id = <your client id>` (what app the user is granting access too)
- `redirect_uri = <your redirect uri>` (which server endpoint to redirect to)
- `scope = <list of scopes>` (what to grant access to)
- `state = <anything you want>` (store info to pass to the server)

## Access Token

Once the user grants access to the application, the authorization server will redirect to the provided URI callback with a code.

The code can be exchanged for an access token by making a POST request to the authorization server with the following information:

- `grant_type = authorization_code`
- `code = <the code you received>`
- `redirect_uri = REDIRECT_URI` (must match URI provided by client)
- `client_id = <your client id>` (which application is making the request)
- `client_secret = <your client secret>` authenticates that the requesting application  is the same application registered with the client ID
- Once granted, the token can be used to make API calls to the service on behalf of the user

---

## Reference Links:

[OAuth 2 Simplified](https://aaronparecki.com/oauth-2-simplified/)

[Video: What is OAuth really all about](https://www.youtube.com/watch?v=t4-416mg6iU)

---

[Home](https://jchinzi.github.io/reading-notes/)