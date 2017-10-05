
# JaxNode October 2017 express demo

This is a set of examples for the JaxNode October 2017 express demo. Express.js is probably the most common web application framework in the Node.js ecosystem.
A web application can be constructed with very few lines of code, as per below;

```Javascript
const express = require('express');
const app = express();
const http = require('http');

app.get('/', (req, res) => {
    res.send('Hello World!');
});

const server = http.createServer(app);
server.listen(3000);
``` 

## Express Middleware
Most of the real power of Express comes from its Middleware. Developers have the option of adding middleware only when it is absolutely required.