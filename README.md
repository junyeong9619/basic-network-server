# Basic Network Server

A Basic Network Server Example using Node's `net` module
```javascript
const server = require('net').createServer();
server.on('connection', socket => {
    // Register a connection handler that fires every time a client connects to this server
    // The handler also gives us access to a connected socket itself
});

server.listen(8000, () => console.log('Server bound'));
```



## To Run The Server
`node net.js`

## To Connect The Server
Use either `telnet` or `nc` to connect to the server<br />
E.g. `nc localhost 8000`
<br />
<br />

**_*From Pluralsight Course with Samer Buna_**
