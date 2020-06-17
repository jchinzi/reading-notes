## [Local Storage](http://diveinto.html5doctor.com/storage.html)

Cookies have three potentially serious downsides when used for persistent local storage:

- The are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

- This also means that cookies send data unencrypted over the internet

- Finally, they are limited to ~4KB of data, which can slow down applications and is generally limiting

Pre-HTML5, there was no good solution to local storage that was spacious and persistant that didn't transmit to the server.

HTML5 sought to provide a standardized API, implemented natively and consistently in multiple browsers, without having to rely on third-party plugins.

HTML5 Storage is a way for web pages to store named key/value pairs locally, within the client web browser.

- HTML5 Storage is accessed through the localStorage object

- The named key is a string.  The data can be any type, but will also be stored as a string.

- Changes to the storage area can be tracked by trapping the *storage* event object, which includes the key, oldValue, newValue and URL.



---
[Home](https://jchinzi.github.io/reading-notes/)