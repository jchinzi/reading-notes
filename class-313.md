## [Sending Form Data](https://developer.mozilla.org/en-US/docs/Learn/Forms/Sending_and_retrieving_form_data)

### Client/Server Architecture

Overview: a client (such as a web browser) sends a request to a server using the HTTP protocol.  The server answers the request using the same protocol.

An HTML form is a user-friendly way to configure that HTTP request.  `<form>` elements define how the data will be sent

- **Action** defines where the data gets sent.  The value must be a valid relative or absolute URL

- **Method** defines how data is sent (usually GET or POST)

  - **GET Method** is used by the browser to ask the server to send back a given resource.  The browser sends an empty body with this method, so if a form is sent  it is appended to the URL

  - **POST Method** is used to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request (including data from forms)
    - POST is therefore preferable for secure data (like passwords) and large amounts of data

### On the Server Side: Retrieving the Data

- The server will receive a string that will be parsed in order to get the data as a list of key/value pairs.  One can access the list directly, but more commonly will use a framework such as *Express*

### A Special Case: Sending Files

- Files are binary data rather than text data

- **Enctype Attribute** lets you specify the value of the *Content-Type* HTTP header included in the request

To send a file:

1. Set **method** to POST (files cannot be put inside a URL)
1. Set value of **enctype** to *multipart/form-data*
1. Include one or more `<input type="file">` controls

### Security Issues

- Issues come from how the server handles data
- [This Article](https://developer.mozilla.org/en-US/docs/Learn/Server-side/First_steps/Website_security) has more details regarding common attacks and potential defences

Good Practices Include:
- Escape potentially dangerous characters (executable code)
- Limit the incoming amount of data to allow only what is necessary
- Sandbox uploaded files (store them on a different server and allow access to the file through different subdomains at the very least)

---

[Home](https://jchinzi.github.io/reading-notes/)