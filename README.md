# Readme
A note about HTTP Caching.

### **If-Modified-Since**/**Last-Modified**

Client request:
- **If-Modified-Since**: \<Last-Modified\>

Server response:
- **200 OK**, with a body, and **Last-Modified**: \<Last-Modified\>
- **304 Not Modified**, without a body

注意**If-Modified-Since**和**Last-Modified**使用GMT时间。

### **If-None-Match**/**ETag**

Client request:
- **If-None-Match**: \<ETag\>

Server response:
- **200 OK**, with a body, and **ETag**: \<ETag\>
- **304 Not Modified**, without a body

注意是**If-None-Match**而不是~~If-Not-Match~~，这是因为**If-None-Match**被设计成可以同时接收多个ETag作为参数。

### **Expires**

Server response:
- **Expires**: \<Expires\>

注意**Expires**使用GMT时间。

### Credits
- Computer Networking: A Top-Down Approach, Eighth Edition
- [If-None-Match - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/If-None-Match)
- [If-Modified-Since - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/If-Modified-Since)
- [Expires - MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Expires)
