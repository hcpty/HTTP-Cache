# Readme
A note about HTTP Caching.

### *If-None-Match*/*ETag*

Client request:
- *If-None-Match*: \<ETag\>

Server response:
- *200 OK*, with a body, and *ETag*: \<ETag\>
- *304 Not Modified*, without a body

### *If-Modified-Since*/*Last-Modified*

Client request:
- *If-Modified-Since*: \<Last-Modified\>

Server response:
- *200 OK*, with a body, and *Last-Modified*: \<Last-Modified\>
- *304 Not Modified*, without a body

### *Expires*

Server response:
- *Expires*: \<Expires\>

### Credits
- Computer Networking: A Top-Down Approach, Eighth Edition
- [If-None-Match - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/If-None-Match)
- [If-Modified-Since - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/If-Modified-Since)
- [Expires - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Expires)
