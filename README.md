# Readme
A note about HTTP Caching.

### ETag/If-None-Match

Client request:
- If-None-Match: \<ETag\>

Server response:
- 200 OK, the latest version of the resource, and the ETag
- 304 Not Modified, without a body

### Credits
- Computer Networking: A Top-Down Approach, Eighth Edition
- [ETag - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/ETag)
