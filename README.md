# api documentation for  [socket.io (v1.7.3)](https://github.com/socketio/socket.io#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-socket.io.svg)](https://travis-ci.org/npmdoc/node-npmdoc-socket.io)
#### node.js realtime framework server

[![NPM](https://nodei.co/npm/socket.io.png?downloads=true)](https://www.npmjs.com/package/socket.io)

[![apidoc](https://npmdoc.github.io/node-npmdoc-socket.io/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-socket.io_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-socket.io/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-socket.io/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "bugs": {
        "url": "https://github.com/socketio/socket.io/issues"
    },
    "contributors": [
        {
            "name": "Guillermo Rauch",
            "email": "rauchg@gmail.com"
        },
        {
            "name": "Arnout Kazemier",
            "email": "info@3rd-eden.com"
        },
        {
            "name": "Vladimir Dronnikov",
            "email": "dronnikov@gmail.com"
        },
        {
            "name": "Einar Otto Stangvik",
            "email": "einaros@gmail.com"
        }
    ],
    "dependencies": {
        "debug": "2.3.3",
        "engine.io": "1.8.3",
        "has-binary": "0.1.7",
        "object-assign": "4.1.0",
        "socket.io-adapter": "0.5.0",
        "socket.io-client": "1.7.3",
        "socket.io-parser": "2.3.1"
    },
    "description": "node.js realtime framework server",
    "devDependencies": {
        "babel-preset-es2015": "6.3.13",
        "del": "2.2.0",
        "expect.js": "0.3.1",
        "gulp": "3.9.0",
        "gulp-babel": "6.1.1",
        "gulp-istanbul": "0.10.3",
        "gulp-mocha": "2.2.0",
        "gulp-task-listing": "1.0.1",
        "istanbul": "0.4.1",
        "mocha": "2.3.4",
        "superagent": "1.6.1",
        "supertest": "1.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "b8af9caba00949e568e369f1327ea9be9ea2461b",
        "tarball": "https://registry.npmjs.org/socket.io/-/socket.io-1.7.3.tgz"
    },
    "files": [
        "lib/"
    ],
    "gitHead": "06044efbe2c6f7bbe8f8a5468e3f04e9fcaa5758",
    "homepage": "https://github.com/socketio/socket.io#readme",
    "keywords": [
        "realtime",
        "framework",
        "websocket",
        "tcp",
        "events",
        "socket",
        "io"
    ],
    "license": "MIT",
    "main": "./lib/index",
    "maintainers": [
        {
            "name": "darrachequesne",
            "email": "damien.arrachequesne@gmail.com"
        },
        {
            "name": "rauchg",
            "email": "rauchg@gmail.com"
        }
    ],
    "name": "socket.io",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/socketio/socket.io.git"
    },
    "scripts": {
        "test": "gulp test"
    },
    "version": "1.7.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module socket.io](#apidoc.module.socket.io)
1.  [function <span class="apidocSignatureSpan">socket.io.</span>io.client (server, conn)](#apidoc.element.socket.io.io.client)
1.  [function <span class="apidocSignatureSpan">socket.io.</span>io.namespace (server, name)](#apidoc.element.socket.io.io.namespace)
1.  [function <span class="apidocSignatureSpan">socket.io.</span>io.socket (nsp, client, query)](#apidoc.element.socket.io.io.socket)
1.  [function <span class="apidocSignatureSpan">socket.io.</span>listen (srv, opts)](#apidoc.element.socket.io.listen)
1.  object <span class="apidocSignatureSpan">socket.io.</span>io.client.prototype
1.  object <span class="apidocSignatureSpan">socket.io.</span>io.namespace.prototype
1.  object <span class="apidocSignatureSpan">socket.io.</span>io.socket.prototype

#### [module socket.io.client](#apidoc.module.socket.io.client)
1.  [function <span class="apidocSignatureSpan">socket.io.</span>client (server, conn)](#apidoc.element.socket.io.client.client)

#### [module socket.io.client.prototype](#apidoc.module.socket.io.client.prototype)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>close ()](#apidoc.element.socket.io.client.prototype.close)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>connect (name, query)](#apidoc.element.socket.io.client.prototype.connect)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>destroy ()](#apidoc.element.socket.io.client.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>disconnect ()](#apidoc.element.socket.io.client.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>onclose (reason)](#apidoc.element.socket.io.client.prototype.onclose)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>ondata (data)](#apidoc.element.socket.io.client.prototype.ondata)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>ondecoded (packet)](#apidoc.element.socket.io.client.prototype.ondecoded)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>onerror (err)](#apidoc.element.socket.io.client.prototype.onerror)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>packet (packet, opts)](#apidoc.element.socket.io.client.prototype.packet)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>remove (socket)](#apidoc.element.socket.io.client.prototype.remove)
1.  [function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>setup ()](#apidoc.element.socket.io.client.prototype.setup)

#### [module socket.io.namespace](#apidoc.module.socket.io.namespace)
1.  [function <span class="apidocSignatureSpan">socket.io.</span>namespace (server, name)](#apidoc.element.socket.io.namespace.namespace)
1.  object <span class="apidocSignatureSpan">socket.io.namespace.</span>events
1.  object <span class="apidocSignatureSpan">socket.io.namespace.</span>flags

#### [module socket.io.namespace.prototype](#apidoc.module.socket.io.namespace.prototype)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>add (client, query, fn)](#apidoc.element.socket.io.namespace.prototype.add)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>clients (fn)](#apidoc.element.socket.io.namespace.prototype.clients)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>compress (compress)](#apidoc.element.socket.io.namespace.prototype.compress)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>emit (ev)](#apidoc.element.socket.io.namespace.prototype.emit)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>in (name)](#apidoc.element.socket.io.namespace.prototype.in)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>initAdapter ()](#apidoc.element.socket.io.namespace.prototype.initAdapter)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>remove (socket)](#apidoc.element.socket.io.namespace.prototype.remove)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>run (socket, fn)](#apidoc.element.socket.io.namespace.prototype.run)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>send ()](#apidoc.element.socket.io.namespace.prototype.send)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>to (name)](#apidoc.element.socket.io.namespace.prototype.to)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>use (fn)](#apidoc.element.socket.io.namespace.prototype.use)
1.  [function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>write ()](#apidoc.element.socket.io.namespace.prototype.write)

#### [module socket.io.socket](#apidoc.module.socket.io.socket)
1.  [function <span class="apidocSignatureSpan">socket.io.</span>socket (nsp, client, query)](#apidoc.element.socket.io.socket.socket)
1.  object <span class="apidocSignatureSpan">socket.io.socket.</span>events

#### [module socket.io.socket.prototype](#apidoc.module.socket.io.socket.prototype)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>ack (id)](#apidoc.element.socket.io.socket.prototype.ack)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>buildHandshake (query)](#apidoc.element.socket.io.socket.prototype.buildHandshake)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>compress (compress)](#apidoc.element.socket.io.socket.prototype.compress)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>disconnect (close)](#apidoc.element.socket.io.socket.prototype.disconnect)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>dispatch (event)](#apidoc.element.socket.io.socket.prototype.dispatch)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>emit (ev)](#apidoc.element.socket.io.socket.prototype.emit)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>error (err)](#apidoc.element.socket.io.socket.prototype.error)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>in (name)](#apidoc.element.socket.io.socket.prototype.in)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>join (room, fn)](#apidoc.element.socket.io.socket.prototype.join)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>leave (room, fn)](#apidoc.element.socket.io.socket.prototype.leave)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>leaveAll ()](#apidoc.element.socket.io.socket.prototype.leaveAll)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onack (packet)](#apidoc.element.socket.io.socket.prototype.onack)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onclose (reason)](#apidoc.element.socket.io.socket.prototype.onclose)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onconnect ()](#apidoc.element.socket.io.socket.prototype.onconnect)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>ondisconnect ()](#apidoc.element.socket.io.socket.prototype.ondisconnect)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onerror (err)](#apidoc.element.socket.io.socket.prototype.onerror)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onevent (packet)](#apidoc.element.socket.io.socket.prototype.onevent)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onpacket (packet)](#apidoc.element.socket.io.socket.prototype.onpacket)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>packet (packet, opts)](#apidoc.element.socket.io.socket.prototype.packet)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>run (event, fn)](#apidoc.element.socket.io.socket.prototype.run)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>send ()](#apidoc.element.socket.io.socket.prototype.send)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>to (name)](#apidoc.element.socket.io.socket.prototype.to)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>use (fn)](#apidoc.element.socket.io.socket.prototype.use)
1.  [function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>write ()](#apidoc.element.socket.io.socket.prototype.write)



# <a name="apidoc.module.socket.io"></a>[module socket.io](#apidoc.module.socket.io)

#### <a name="apidoc.element.socket.io.io.client"></a>[function <span class="apidocSignatureSpan">socket.io.</span>io.client (server, conn)](#apidoc.element.socket.io.io.client)
- description and source-code
```javascript
function Client(server, conn){
  this.server = server;
  this.conn = conn;
  this.encoder = new parser.Encoder();
  this.decoder = new parser.Decoder();
  this.id = conn.id;
  this.request = conn.request;
  this.setup();
  this.sockets = {};
  this.nsps = {};
  this.connectBuffer = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.io.namespace"></a>[function <span class="apidocSignatureSpan">socket.io.</span>io.namespace (server, name)](#apidoc.element.socket.io.io.namespace)
- description and source-code
```javascript
function Namespace(server, name){
  this.name = name;
  this.server = server;
  this.sockets = {};
  this.connected = {};
  this.fns = [];
  this.ids = 0;
  this.initAdapter();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.io.socket"></a>[function <span class="apidocSignatureSpan">socket.io.</span>io.socket (nsp, client, query)](#apidoc.element.socket.io.io.socket)
- description and source-code
```javascript
function Socket(nsp, client, query){
  this.nsp = nsp;
  this.server = nsp.server;
  this.adapter = this.nsp.adapter;
  this.id = nsp.name !== '/' ? nsp.name + '#' + client.id : client.id;
  this.client = client;
  this.conn = client.conn;
  this.rooms = {};
  this.acks = {};
  this.connected = true;
  this.disconnected = false;
  this.handshake = this.buildHandshake(query);
  this.fns = [];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.listen"></a>[function <span class="apidocSignatureSpan">socket.io.</span>listen (srv, opts)](#apidoc.element.socket.io.listen)
- description and source-code
```javascript
function Server(srv, opts){
  if (!(this instanceof Server)) return new Server(srv, opts);
  if ('object' == typeof srv && !srv.listen) {
    opts = srv;
    srv = null;
  }
  opts = opts || {};
  this.nsps = {};
  this.path(opts.path || '/socket.io');
  this.serveClient(false !== opts.serveClient);
  this.adapter(opts.adapter || Adapter);
  this.origins(opts.origins || '*:*');
  this.sockets = this.of('/');
  if (srv) this.attach(srv, opts);
}
```
- example usage
```shell
...
'''js
var server = require('http').createServer();
var io = require('socket.io')(server);
io.on('connection', function(client){
  client.on('event', function(data){});
  client.on('disconnect', function(){});
});
server.listen(3000);
'''

### Standalone

'''js
var io = require('socket.io')();
io.on('connection', function(client){});
...
```



# <a name="apidoc.module.socket.io.client"></a>[module socket.io.client](#apidoc.module.socket.io.client)

#### <a name="apidoc.element.socket.io.client.client"></a>[function <span class="apidocSignatureSpan">socket.io.</span>client (server, conn)](#apidoc.element.socket.io.client.client)
- description and source-code
```javascript
function Client(server, conn){
  this.server = server;
  this.conn = conn;
  this.encoder = new parser.Encoder();
  this.decoder = new parser.Decoder();
  this.id = conn.id;
  this.request = conn.request;
  this.setup();
  this.sockets = {};
  this.nsps = {};
  this.connectBuffer = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io.client.prototype"></a>[module socket.io.client.prototype](#apidoc.module.socket.io.client.prototype)

#### <a name="apidoc.element.socket.io.client.prototype.close"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>close ()](#apidoc.element.socket.io.client.prototype.close)
- description and source-code
```javascript
close = function (){
  if ('open' == this.conn.readyState) {
    debug('forcing transport close');
    this.conn.close();
    this.onclose('forced server close');
  }
}
```
- example usage
```shell
...

For other available methods, see 'Namespace' below.

### Server#close([fn:Function])

Closes socket.io server.

The optional 'fn' is passed to the 'server.close([callback])' method of the
core 'net' module and is called on error or when all connections are closed.
The callback is expected to implement the common single argument 'err'
signature (if any).

'''js
var Server = require('socket.io');
var PORT   = 3030;
...
```

#### <a name="apidoc.element.socket.io.client.prototype.connect"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>connect (name, query)](#apidoc.element.socket.io.client.prototype.connect)
- description and source-code
```javascript
connect = function (name, query){
  debug('connecting to namespace %s', name);
  var nsp = this.server.nsps[name];
  if (!nsp) {
    this.packet({ type: parser.ERROR, nsp: name, data : 'Invalid namespace'});
    return;
  }

  if ('/' != name && !this.nsps['/']) {
    this.connectBuffer.push(name);
    return;
  }

  var self = this;
  var socket = nsp.add(this, query, function(){
    self.sockets[socket.id] = socket;
    self.nsps[nsp.name] = socket;

    if ('/' == nsp.name && self.connectBuffer.length > 0) {
      self.connectBuffer.forEach(self.connect, self);
      self.connectBuffer = [];
    }
  });
}
```
- example usage
```shell
...
 * Called when parser fully decodes a packet.
 *
 * @api private
 */

Client.prototype.ondecoded = function(packet) {
if (parser.CONNECT == packet.type) {
  this.connect(url.parse(packet.nsp).pathname, url.parse(packet.nsp, true).query);
} else {
  var socket = this.nsps[packet.nsp];
  if (socket) {
    process.nextTick(function() {
      socket.onpacket(packet);
    });
  } else {
...
```

#### <a name="apidoc.element.socket.io.client.prototype.destroy"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>destroy ()](#apidoc.element.socket.io.client.prototype.destroy)
- description and source-code
```javascript
destroy = function (){
  this.conn.removeListener('data', this.ondata);
  this.conn.removeListener('error', this.onerror);
  this.conn.removeListener('close', this.onclose);
  this.decoder.removeListener('decoded', this.ondecoded);
}
```
- example usage
```shell
...
 * @api private
 */

Client.prototype.onclose = function(reason){
debug('client close with reason %s', reason);

// ignore a potential subsequent 'close' event
this.destroy();

// 'nsps' and 'sockets' are cleaned up seamlessly
for (var id in this.sockets) {
  if (this.sockets.hasOwnProperty(id)) {
    this.sockets[id].onclose(reason);
  }
}
...
```

#### <a name="apidoc.element.socket.io.client.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>disconnect ()](#apidoc.element.socket.io.client.prototype.disconnect)
- description and source-code
```javascript
disconnect = function (){
  for (var id in this.sockets) {
    if (this.sockets.hasOwnProperty(id)) {
      this.sockets[id].disconnect();
    }
  }
  this.sockets = {};
  this.close();
}
```
- example usage
```shell
...
 *
 * @api private
 */

Client.prototype.disconnect = function(){
  for (var id in this.sockets) {
    if (this.sockets.hasOwnProperty(id)) {
      this.sockets[id].disconnect();
    }
  }
  this.sockets = {};
  this.close();
};

/**
...
```

#### <a name="apidoc.element.socket.io.client.prototype.onclose"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>onclose (reason)](#apidoc.element.socket.io.client.prototype.onclose)
- description and source-code
```javascript
onclose = function (reason){
  debug('client close with reason %s', reason);

  // ignore a potential subsequent 'close' event
  this.destroy();

  // 'nsps' and 'sockets' are cleaned up seamlessly
  for (var id in this.sockets) {
    if (this.sockets.hasOwnProperty(id)) {
      this.sockets[id].onclose(reason);
    }
  }
  this.sockets = {};

  this.decoder.destroy(); // clean up decoder
}
```
- example usage
```shell
...
* @api private
*/

Client.prototype.close = function(){
 if ('open' == this.conn.readyState) {
   debug('forcing transport close');
   this.conn.close();
   this.onclose('forced server close');
 }
};

/**
* Writes a packet to the transport.
*
* @param {Object} packet object
...
```

#### <a name="apidoc.element.socket.io.client.prototype.ondata"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>ondata (data)](#apidoc.element.socket.io.client.prototype.ondata)
- description and source-code
```javascript
ondata = function (data){
  // try/catch is needed for protocol violations (GH-1880)
  try {
    this.decoder.add(data);
  } catch(e) {
    this.onerror(e);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.client.prototype.ondecoded"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>ondecoded (packet)](#apidoc.element.socket.io.client.prototype.ondecoded)
- description and source-code
```javascript
ondecoded = function (packet) {
  if (parser.CONNECT == packet.type) {
    this.connect(url.parse(packet.nsp).pathname, url.parse(packet.nsp, true).query);
  } else {
    var socket = this.nsps[packet.nsp];
    if (socket) {
      process.nextTick(function() {
        socket.onpacket(packet);
      });
    } else {
      debug('no socket for namespace %s', packet.nsp);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.client.prototype.onerror"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>onerror (err)](#apidoc.element.socket.io.client.prototype.onerror)
- description and source-code
```javascript
onerror = function (err){
  for (var id in this.sockets) {
    if (this.sockets.hasOwnProperty(id)) {
      this.sockets[id].onerror(err);
    }
  }
  this.onclose('client error');
}
```
- example usage
```shell
...
*/

Client.prototype.ondata = function(data){
 // try/catch is needed for protocol violations (GH-1880)
 try {
   this.decoder.add(data);
 } catch(e) {
   this.onerror(e);
 }
};

/**
* Called when parser fully decodes a packet.
*
* @api private
...
```

#### <a name="apidoc.element.socket.io.client.prototype.packet"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>packet (packet, opts)](#apidoc.element.socket.io.client.prototype.packet)
- description and source-code
```javascript
packet = function (packet, opts){
  opts = opts || {};
  var self = this;

  // this writes to the actual connection
  function writeToEngine(encodedPackets) {
    if (opts.volatile && !self.conn.transport.writable) return;
    for (var i = 0; i < encodedPackets.length; i++) {
      self.conn.write(encodedPackets[i], { compress: opts.compress });
    }
  }

  if ('open' == this.conn.readyState) {
    debug('writing packet %j', packet);
    if (!opts.preEncoded) { // not broadcasting, need to encode
      this.encoder.encode(packet, function (encodedPackets) { // encode, then write results to engine
        writeToEngine(encodedPackets);
      });
    } else { // a broadcast pre-encodes a packet
      writeToEngine(packet);
    }
  } else {
    debug('ignoring packet write %j', packet);
  }
}
```
- example usage
```shell
...
 * @api private
 */

Client.prototype.connect = function(name, query){
debug('connecting to namespace %s', name);
var nsp = this.server.nsps[name];
if (!nsp) {
  this.packet({ type: parser.ERROR, nsp: name, data : 'Invalid namespace'});
  return;
}

if ('/' != name && !this.nsps['/']) {
  this.connectBuffer.push(name);
  return;
}
...
```

#### <a name="apidoc.element.socket.io.client.prototype.remove"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>remove (socket)](#apidoc.element.socket.io.client.prototype.remove)
- description and source-code
```javascript
remove = function (socket){
  if (this.sockets.hasOwnProperty(socket.id)) {
    var nsp = this.sockets[socket.id].nsp.name;
    delete this.sockets[socket.id];
    delete this.nsps[nsp];
  } else {
    debug('ignoring remove for %s', socket.id);
  }
}
```
- example usage
```shell
...
 */

Socket.prototype.onclose = function(reason){
  if (!this.connected) return this;
  debug('closing socket - reason %s', reason);
  this.emit('disconnecting', reason);
  this.leaveAll();
  this.nsp.remove(this);
  this.client.remove(this);
  this.connected = false;
  this.disconnected = true;
  delete this.nsp.connected[this.id];
  this.emit('disconnect', reason);
};
...
```

#### <a name="apidoc.element.socket.io.client.prototype.setup"></a>[function <span class="apidocSignatureSpan">socket.io.client.prototype.</span>setup ()](#apidoc.element.socket.io.client.prototype.setup)
- description and source-code
```javascript
setup = function (){
  this.onclose = this.onclose.bind(this);
  this.ondata = this.ondata.bind(this);
  this.onerror = this.onerror.bind(this);
  this.ondecoded = this.ondecoded.bind(this);

  this.decoder.on('decoded', this.ondecoded);
  this.conn.on('data', this.ondata);
  this.conn.on('error', this.onerror);
  this.conn.on('close', this.onclose);
}
```
- example usage
```shell
...
function Client(server, conn){
 this.server = server;
 this.conn = conn;
 this.encoder = new parser.Encoder();
 this.decoder = new parser.Decoder();
 this.id = conn.id;
 this.request = conn.request;
 this.setup();
 this.sockets = {};
 this.nsps = {};
 this.connectBuffer = [];
}

/**
* Sets up event listeners.
...
```



# <a name="apidoc.module.socket.io.namespace"></a>[module socket.io.namespace](#apidoc.module.socket.io.namespace)

#### <a name="apidoc.element.socket.io.namespace.namespace"></a>[function <span class="apidocSignatureSpan">socket.io.</span>namespace (server, name)](#apidoc.element.socket.io.namespace.namespace)
- description and source-code
```javascript
function Namespace(server, name){
  this.name = name;
  this.server = server;
  this.sockets = {};
  this.connected = {};
  this.fns = [];
  this.ids = 0;
  this.initAdapter();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io.namespace.prototype"></a>[module socket.io.namespace.prototype](#apidoc.module.socket.io.namespace.prototype)

#### <a name="apidoc.element.socket.io.namespace.prototype.add"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>add (client, query, fn)](#apidoc.element.socket.io.namespace.prototype.add)
- description and source-code
```javascript
add = function (client, query, fn){
  debug('adding socket to nsp %s', this.name);
  var socket = new Socket(this, client, query);
  var self = this;
  this.run(socket, function(err){
    process.nextTick(function(){
      if ('open' == client.conn.readyState) {
        if (err) return socket.error(err.data || err.message);

        // track socket
        self.sockets[socket.id] = socket;

        // it's paramount that the internal 'onconnect' logic
        // fires before user-set events to prevent state order
        // violations (such as a disconnection before the connection
        // logic is complete)
        socket.onconnect();
        if (fn) fn();

        // fire user-set events
        self.emit('connect', socket);
        self.emit('connection', socket);
      } else {
        debug('next called after client was closed - ignoring socket');
      }
    });
  });
  return socket;
}
```
- example usage
```shell
...

  if ('/' != name && !this.nsps['/']) {
this.connectBuffer.push(name);
return;
  }

  var self = this;
  var socket = nsp.add(this, query, function(){
self.sockets[socket.id] = socket;
self.nsps[nsp.name] = socket;

if ('/' == nsp.name && self.connectBuffer.length > 0) {
  self.connectBuffer.forEach(self.connect, self);
  self.connectBuffer = [];
}
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.clients"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>clients (fn)](#apidoc.element.socket.io.namespace.prototype.clients)
- description and source-code
```javascript
clients = function (fn){
  this.adapter.clients(this.rooms, fn);
  // delete rooms flag for scenario:
  // .in('room').clients() (GH-1978)
  delete this.rooms;
  return this;
}
```
- example usage
```shell
...

Gets a list of client IDs connected to this namespace (across all nodes if applicable).

An example to get all clients in a namespace:

'''js
var io = require('socket.io')();
io.of('/chat').clients(function(error, clients){
  if (error) throw error;
  console.log(clients); // => [PZDoMHjiu8PYfRiKAAAF, Anw2LatarvGVVXEIAAAD]
});
'''

An example to get all clients in namespace's room:
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.compress"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>compress (compress)](#apidoc.element.socket.io.namespace.prototype.compress)
- description and source-code
```javascript
compress = function (compress){
  this.flags = this.flags || {};
  this.flags.compress = compress;
  return this;
}
```
- example usage
```shell
...

Sets a modifier for a subsequent event emission that the event data will
only be _compressed_ if the value is 'true'. Defaults to 'true' when you don't call the method.

'''js
var io = require('socket.io')();
io.on('connection', function(client){
  client.compress(false).emit('an event', { some: 'data' });
});
'''

### Socket#disconnect(close:Boolean):Socket

Disconnects this client. If value of close is 'true', closes the underlying connection.
Otherwise, it just disconnects the namespace.
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.emit"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>emit (ev)](#apidoc.element.socket.io.namespace.prototype.emit)
- description and source-code
```javascript
emit = function (ev){
  if (~exports.events.indexOf(ev)) {
    emit.apply(this, arguments);
  } else {
    // set up packet object
    var args = Array.prototype.slice.call(arguments);
    var parserType = parser.EVENT; // default
    if (hasBin(args)) { parserType = parser.BINARY_EVENT; } // binary

    var packet = { type: parserType, data: args };

    if ('function' == typeof args[args.length - 1]) {
      throw new Error('Callbacks are not supported when broadcasting');
    }

    this.adapter.broadcast(packet, {
      rooms: this.rooms,
      flags: this.flags
    });

    delete this.rooms;
    delete this.flags;
  }
  return this;
}
```
- example usage
```shell
...
### Server#emit

  Emits an event to all connected clients. The following two are
  equivalent:

  '''js
  var io = require('socket.io')();
  io.sockets.emit('an event sent to all connected clients');
  io.emit('an event sent to all connected clients');
  '''

  For other available methods, see 'Namespace' below.

### Server#close([fn:Function])
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.in"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>in (name)](#apidoc.element.socket.io.namespace.prototype.in)
- description and source-code
```javascript
in = function (name){
  this.rooms = this.rooms || [];
  if (!~this.rooms.indexOf(name)) this.rooms.push(name);
  return this;
}
```
- example usage
```shell
...
});
'''

An example to get all clients in namespace's room:

'''js
var io = require('socket.io')();
io.of('/chat').in('general').clients(function(error, clients){
  if (error) throw error;
  console.log(clients); // => [Anw2LatarvGVVXEIAAAD]
});
'''

As with broadcasting, the default is all clients from the default namespace ('/'):
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.initAdapter"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>initAdapter ()](#apidoc.element.socket.io.namespace.prototype.initAdapter)
- description and source-code
```javascript
initAdapter = function (){
  this.adapter = new (this.server.adapter())(this);
}
```
- example usage
```shell
...
function Namespace(server, name){
  this.name = name;
  this.server = server;
  this.sockets = {};
  this.connected = {};
  this.fns = [];
  this.ids = 0;
  this.initAdapter();
}

/**
 * Inherits from 'EventEmitter'.
 */

Namespace.prototype.__proto__ = Emitter.prototype;
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.remove"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>remove (socket)](#apidoc.element.socket.io.namespace.prototype.remove)
- description and source-code
```javascript
remove = function (socket){
  if (this.sockets.hasOwnProperty(socket.id)) {
    delete this.sockets[socket.id];
  } else {
    debug('ignoring remove for %s', socket.id);
  }
}
```
- example usage
```shell
...
 */

Socket.prototype.onclose = function(reason){
  if (!this.connected) return this;
  debug('closing socket - reason %s', reason);
  this.emit('disconnecting', reason);
  this.leaveAll();
  this.nsp.remove(this);
  this.client.remove(this);
  this.connected = false;
  this.disconnected = true;
  delete this.nsp.connected[this.id];
  this.emit('disconnect', reason);
};
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.run"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>run (socket, fn)](#apidoc.element.socket.io.namespace.prototype.run)
- description and source-code
```javascript
run = function (socket, fn){
  var fns = this.fns.slice(0);
  if (!fns.length) return fn(null);

  function run(i){
    fns[i](socket, function(err){
      // upon error, short-circuit
      if (err) return fn(err);

      // if no middleware left, summon callback
      if (!fns[i + 1]) return fn(null);

      // go on to next
      run(i + 1);
    });
  }

  run(0);
}
```
- example usage
```shell
...
 * @api private
 */

Namespace.prototype.add = function(client, query, fn){
  debug('adding socket to nsp %s', this.name);
  var socket = new Socket(this, client, query);
  var self = this;
  this.run(socket, function(err){
    process.nextTick(function(){
      if ('open' == client.conn.readyState) {
if (err) return socket.error(err.data || err.message);

// track socket
self.sockets[socket.id] = socket;
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.send"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>send ()](#apidoc.element.socket.io.namespace.prototype.send)
- description and source-code
```javascript
send = function (){
  var args = Array.prototype.slice.call(arguments);
  args.unshift('message');
  this.emit.apply(this, args);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.namespace.prototype.to"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>to (name)](#apidoc.element.socket.io.namespace.prototype.to)
- description and source-code
```javascript
to = function (name){
  this.rooms = this.rooms || [];
  if (!~this.rooms.indexOf(name)) this.rooms.push(name);
  return this;
}
```
- example usage
```shell
...
only be _broadcasted_ to clients that have joined the given 'room'.

To emit to multiple rooms, you can call 'to' several times.

'''js
var io = require('socket.io')();
io.on('connection', function(client){
  client.to('others').emit('an event', { some: 'data' });
});
'''

### Socket#in(room:String):Socket

Same as 'Socket#to'
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.use"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>use (fn)](#apidoc.element.socket.io.namespace.prototype.use)
- description and source-code
```javascript
use = function (fn){
  this.fns.push(fn);
  return this;
}
```
- example usage
```shell
...
Registers a middleware, which is a function that gets executed for
every incoming 'Socket', and receives as parameters the socket and a
function to optionally defer execution to the next registered
middleware.

'''js
var io = require('socket.io')();
io.use(function(socket, next){
  if (socket.request.headers.cookie) return next();
  next(new Error('Authentication error'));
});
'''

Errors passed to middleware callbacks are sent as special 'error'
packets to clients.
...
```

#### <a name="apidoc.element.socket.io.namespace.prototype.write"></a>[function <span class="apidocSignatureSpan">socket.io.namespace.prototype.</span>write ()](#apidoc.element.socket.io.namespace.prototype.write)
- description and source-code
```javascript
write = function (){
  var args = Array.prototype.slice.call(arguments);
  args.unshift('message');
  this.emit.apply(this, args);
  return this;
}
```
- example usage
```shell
...
opts = opts || {};
var self = this;

// this writes to the actual connection
function writeToEngine(encodedPackets) {
  if (opts.volatile && !self.conn.transport.writable) return;
  for (var i = 0; i < encodedPackets.length; i++) {
    self.conn.write(encodedPackets[i], { compress: opts.compress });
  }
}

if ('open' == this.conn.readyState) {
  debug('writing packet %j', packet);
  if (!opts.preEncoded) { // not broadcasting, need to encode
    this.encoder.encode(packet, function (encodedPackets) { // encode, then write results to engine
...
```



# <a name="apidoc.module.socket.io.socket"></a>[module socket.io.socket](#apidoc.module.socket.io.socket)

#### <a name="apidoc.element.socket.io.socket.socket"></a>[function <span class="apidocSignatureSpan">socket.io.</span>socket (nsp, client, query)](#apidoc.element.socket.io.socket.socket)
- description and source-code
```javascript
function Socket(nsp, client, query){
  this.nsp = nsp;
  this.server = nsp.server;
  this.adapter = this.nsp.adapter;
  this.id = nsp.name !== '/' ? nsp.name + '#' + client.id : client.id;
  this.client = client;
  this.conn = client.conn;
  this.rooms = {};
  this.acks = {};
  this.connected = true;
  this.disconnected = false;
  this.handshake = this.buildHandshake(query);
  this.fns = [];
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.socket.io.socket.prototype"></a>[module socket.io.socket.prototype](#apidoc.module.socket.io.socket.prototype)

#### <a name="apidoc.element.socket.io.socket.prototype.ack"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>ack (id)](#apidoc.element.socket.io.socket.prototype.ack)
- description and source-code
```javascript
ack = function (id){
  var self = this;
  var sent = false;
  return function(){
    // prevent double callbacks
    if (sent) return;
    var args = Array.prototype.slice.call(arguments);
    debug('sending ack %j', args);

    var type = hasBin(args) ? parser.BINARY_ACK : parser.ACK;
    self.packet({
      id: id,
      type: type,
      data: args
    });

    sent = true;
  };
}
```
- example usage
```shell
...

Socket.prototype.onevent = function(packet){
 var args = packet.data || [];
 debug('emitting event %j', args);

 if (null != packet.id) {
   debug('attaching ack callback to event');
   args.push(this.ack(packet.id));
 }

 this.dispatch(args);
};

/**
* Produces an ack callback to emit with an event.
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.buildHandshake"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>buildHandshake (query)](#apidoc.element.socket.io.socket.prototype.buildHandshake)
- description and source-code
```javascript
buildHandshake = function (query){
  var self = this;
  function buildQuery(){
    var requestQuery = url.parse(self.request.url, true).query;
    //if socket-specific query exist, replace query strings in requestQuery
    return assign({}, query, requestQuery);
  }
  return {
    headers: this.request.headers,
    time: (new Date) + '',
    address: this.conn.remoteAddress,
    xdomain: !!this.request.headers.origin,
    secure: !!this.request.connection.encrypted,
    issued: +(new Date),
    url: this.request.url,
    query: buildQuery()
  };
}
```
- example usage
```shell
...
 this.id = nsp.name !== '/' ? nsp.name + '#' + client.id : client.id;
 this.client = client;
 this.conn = client.conn;
 this.rooms = {};
 this.acks = {};
 this.connected = true;
 this.disconnected = false;
 this.handshake = this.buildHandshake(query);
 this.fns = [];
}

/**
* Inherits from 'EventEmitter'.
*/
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.compress"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>compress (compress)](#apidoc.element.socket.io.socket.prototype.compress)
- description and source-code
```javascript
compress = function (compress){
  this.flags = this.flags || {};
  this.flags.compress = compress;
  return this;
}
```
- example usage
```shell
...

Sets a modifier for a subsequent event emission that the event data will
only be _compressed_ if the value is 'true'. Defaults to 'true' when you don't call the method.

'''js
var io = require('socket.io')();
io.on('connection', function(client){
  client.compress(false).emit('an event', { some: 'data' });
});
'''

### Socket#disconnect(close:Boolean):Socket

Disconnects this client. If value of close is 'true', closes the underlying connection.
Otherwise, it just disconnects the namespace.
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.disconnect"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>disconnect (close)](#apidoc.element.socket.io.socket.prototype.disconnect)
- description and source-code
```javascript
disconnect = function (close){
  if (!this.connected) return this;
  if (close) {
    this.client.disconnect();
  } else {
    this.packet({ type: parser.DISCONNECT });
    this.onclose('server namespace disconnect');
  }
  return this;
}
```
- example usage
```shell
...
 *
 * @api private
 */

Client.prototype.disconnect = function(){
  for (var id in this.sockets) {
    if (this.sockets.hasOwnProperty(id)) {
      this.sockets[id].disconnect();
    }
  }
  this.sockets = {};
  this.close();
};

/**
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.dispatch"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>dispatch (event)](#apidoc.element.socket.io.socket.prototype.dispatch)
- description and source-code
```javascript
dispatch = function (event){
  debug('dispatching an event %j', event);
  var self = this;
  this.run(event, function(err){
    process.nextTick(function(){
      if (err) {
        return self.error(err.data || err.message);
      }
      emit.apply(self, event);
    });
  });
}
```
- example usage
```shell
...
 debug('emitting event %j', args);

 if (null != packet.id) {
   debug('attaching ack callback to event');
   args.push(this.ack(packet.id));
 }

 this.dispatch(args);
};

/**
* Produces an ack callback to emit with an event.
*
* @param {Number} id packet id
* @api private
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.emit"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>emit (ev)](#apidoc.element.socket.io.socket.prototype.emit)
- description and source-code
```javascript
emit = function (ev){
  if (~exports.events.indexOf(ev)) {
    emit.apply(this, arguments);
  } else {
    var args = Array.prototype.slice.call(arguments);
    var packet = {};
    packet.type = hasBin(args) ? parser.BINARY_EVENT : parser.EVENT;
    packet.data = args;
    var flags = this.flags || {};

    // access last argument to see if it's an ACK callback
    if ('function' == typeof args[args.length - 1]) {
      if (this._rooms || flags.broadcast) {
        throw new Error('Callbacks are not supported when broadcasting');
      }

      debug('emitting packet with ack id %d', this.nsp.ids);
      this.acks[this.nsp.ids] = args.pop();
      packet.id = this.nsp.ids++;
    }

    if (this._rooms || flags.broadcast) {
      this.adapter.broadcast(packet, {
        except: [this.id],
        rooms: this._rooms,
        flags: flags
      });
    } else {
      // dispatch packet
      this.packet(packet, {
        volatile: flags.volatile,
        compress: flags.compress
      });
    }

    // reset flags
    delete this._rooms;
    delete this.flags;
  }
  return this;
}
```
- example usage
```shell
...
### Server#emit

  Emits an event to all connected clients. The following two are
  equivalent:

  '''js
  var io = require('socket.io')();
  io.sockets.emit('an event sent to all connected clients');
  io.emit('an event sent to all connected clients');
  '''

  For other available methods, see 'Namespace' below.

### Server#close([fn:Function])
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.error"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>error (err)](#apidoc.element.socket.io.socket.prototype.error)
- description and source-code
```javascript
error = function (err){
  this.packet({ type: parser.ERROR, data: err });
}
```
- example usage
```shell
...
Namespace.prototype.add = function(client, query, fn){
  debug('adding socket to nsp %s', this.name);
  var socket = new Socket(this, client, query);
  var self = this;
  this.run(socket, function(err){
    process.nextTick(function(){
      if ('open' == client.conn.readyState) {
if (err) return socket.error(err.data || err.message);

// track socket
self.sockets[socket.id] = socket;

// it's paramount that the internal 'onconnect' logic
// fires before user-set events to prevent state order
// violations (such as a disconnection before the connection
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.in"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>in (name)](#apidoc.element.socket.io.socket.prototype.in)
- description and source-code
```javascript
in = function (name){
  this._rooms = this._rooms || [];
  if (!~this._rooms.indexOf(name)) this._rooms.push(name);
  return this;
}
```
- example usage
```shell
...
});
'''

An example to get all clients in namespace's room:

'''js
var io = require('socket.io')();
io.of('/chat').in('general').clients(function(error, clients){
  if (error) throw error;
  console.log(clients); // => [Anw2LatarvGVVXEIAAAD]
});
'''

As with broadcasting, the default is all clients from the default namespace ('/'):
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.join"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>join (room, fn)](#apidoc.element.socket.io.socket.prototype.join)
- description and source-code
```javascript
join = function (room, fn){
  debug('joining room %s', room);
  var self = this;
  if (this.rooms.hasOwnProperty(room)) {
    fn && fn(null);
    return this;
  }
  this.adapter.add(this.id, room, function(err){
    if (err) return fn && fn(err);
    debug('joined room %s', room);
    self.rooms[room] = room;
    fn && fn(null);
  });
  return this;
}
```
- example usage
```shell
...
*
* @api private
*/

Socket.prototype.onconnect = function(){
 debug('socket connected - writing packet');
 this.nsp.connected[this.id] = this;
 this.join(this.id);
 this.packet({ type: parser.CONNECT });
};

/**
* Called with each packet. Called by 'Client'.
*
* @param {Object} packet
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.leave"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>leave (room, fn)](#apidoc.element.socket.io.socket.prototype.leave)
- description and source-code
```javascript
leave = function (room, fn){
  debug('leave room %s', room);
  var self = this;
  this.adapter.del(this.id, room, function(err){
    if (err) return fn && fn(err);
    debug('left room %s', room);
    delete self.rooms[room];
    fn && fn(null);
  });
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.socket.prototype.leaveAll"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>leaveAll ()](#apidoc.element.socket.io.socket.prototype.leaveAll)
- description and source-code
```javascript
leaveAll = function (){
  this.adapter.delAll(this.id);
  this.rooms = {};
}
```
- example usage
```shell
...
 * @api private
 */

Socket.prototype.onclose = function(reason){
  if (!this.connected) return this;
  debug('closing socket - reason %s', reason);
  this.emit('disconnecting', reason);
  this.leaveAll();
  this.nsp.remove(this);
  this.client.remove(this);
  this.connected = false;
  this.disconnected = true;
  delete this.nsp.connected[this.id];
  this.emit('disconnect', reason);
};
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.onack"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onack (packet)](#apidoc.element.socket.io.socket.prototype.onack)
- description and source-code
```javascript
onack = function (packet){
  var ack = this.acks[packet.id];
  if ('function' == typeof ack) {
    debug('calling ack %s with %j', packet.id, packet.data);
    ack.apply(this, packet.data);
    delete this.acks[packet.id];
  } else {
    debug('bad ack %s', packet.id);
  }
}
```
- example usage
```shell
...
  break;

case parser.BINARY_EVENT:
  this.onevent(packet);
  break;

case parser.ACK:
  this.onack(packet);
  break;

case parser.BINARY_ACK:
  this.onack(packet);
  break;

case parser.DISCONNECT:
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.onclose"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onclose (reason)](#apidoc.element.socket.io.socket.prototype.onclose)
- description and source-code
```javascript
onclose = function (reason){
  if (!this.connected) return this;
  debug('closing socket - reason %s', reason);
  this.emit('disconnecting', reason);
  this.leaveAll();
  this.nsp.remove(this);
  this.client.remove(this);
  this.connected = false;
  this.disconnected = true;
  delete this.nsp.connected[this.id];
  this.emit('disconnect', reason);
}
```
- example usage
```shell
...
* @api private
*/

Client.prototype.close = function(){
 if ('open' == this.conn.readyState) {
   debug('forcing transport close');
   this.conn.close();
   this.onclose('forced server close');
 }
};

/**
* Writes a packet to the transport.
*
* @param {Object} packet object
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.onconnect"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onconnect ()](#apidoc.element.socket.io.socket.prototype.onconnect)
- description and source-code
```javascript
onconnect = function (){
  debug('socket connected - writing packet');
  this.nsp.connected[this.id] = this;
  this.join(this.id);
  this.packet({ type: parser.CONNECT });
}
```
- example usage
```shell
...
  // track socket
  self.sockets[socket.id] = socket;

  // it's paramount that the internal 'onconnect' logic
  // fires before user-set events to prevent state order
  // violations (such as a disconnection before the connection
  // logic is complete)
  socket.onconnect();
  if (fn) fn();

  // fire user-set events
  self.emit('connect', socket);
  self.emit('connection', socket);
} else {
  debug('next called after client was closed - ignoring socket');
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.ondisconnect"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>ondisconnect ()](#apidoc.element.socket.io.socket.prototype.ondisconnect)
- description and source-code
```javascript
ondisconnect = function (){
  debug('got disconnect packet');
  this.onclose('client namespace disconnect');
}
```
- example usage
```shell
...
      break;

    case parser.BINARY_ACK:
      this.onack(packet);
      break;

    case parser.DISCONNECT:
      this.ondisconnect();
      break;

    case parser.ERROR:
      this.emit('error', packet.data);
  }
};
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.onerror"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onerror (err)](#apidoc.element.socket.io.socket.prototype.onerror)
- description and source-code
```javascript
onerror = function (err){
  if (this.listeners('error').length) {
    this.emit('error', err);
  } else {
    console.error('Missing error handler on 'socket'.');
    console.error(err.stack);
  }
}
```
- example usage
```shell
...
*/

Client.prototype.ondata = function(data){
 // try/catch is needed for protocol violations (GH-1880)
 try {
   this.decoder.add(data);
 } catch(e) {
   this.onerror(e);
 }
};

/**
* Called when parser fully decodes a packet.
*
* @api private
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.onevent"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onevent (packet)](#apidoc.element.socket.io.socket.prototype.onevent)
- description and source-code
```javascript
onevent = function (packet){
  var args = packet.data || [];
  debug('emitting event %j', args);

  if (null != packet.id) {
    debug('attaching ack callback to event');
    args.push(this.ack(packet.id));
  }

  this.dispatch(args);
}
```
- example usage
```shell
...
 * @api private
 */

Socket.prototype.onpacket = function(packet){
  debug('got packet %j', packet);
  switch (packet.type) {
case parser.EVENT:
  this.onevent(packet);
  break;

case parser.BINARY_EVENT:
  this.onevent(packet);
  break;

case parser.ACK:
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.onpacket"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>onpacket (packet)](#apidoc.element.socket.io.socket.prototype.onpacket)
- description and source-code
```javascript
onpacket = function (packet){
  debug('got packet %j', packet);
  switch (packet.type) {
    case parser.EVENT:
      this.onevent(packet);
      break;

    case parser.BINARY_EVENT:
      this.onevent(packet);
      break;

    case parser.ACK:
      this.onack(packet);
      break;

    case parser.BINARY_ACK:
      this.onack(packet);
      break;

    case parser.DISCONNECT:
      this.ondisconnect();
      break;

    case parser.ERROR:
      this.emit('error', packet.data);
  }
}
```
- example usage
```shell
...
Client.prototype.ondecoded = function(packet) {
  if (parser.CONNECT == packet.type) {
    this.connect(url.parse(packet.nsp).pathname, url.parse(packet.nsp, true).query);
  } else {
    var socket = this.nsps[packet.nsp];
    if (socket) {
      process.nextTick(function() {
        socket.onpacket(packet);
      });
    } else {
      debug('no socket for namespace %s', packet.nsp);
    }
  }
};
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.packet"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>packet (packet, opts)](#apidoc.element.socket.io.socket.prototype.packet)
- description and source-code
```javascript
packet = function (packet, opts){
  packet.nsp = this.nsp.name;
  opts = opts || {};
  opts.compress = false !== opts.compress;
  this.client.packet(packet, opts);
}
```
- example usage
```shell
...
 * @api private
 */

Client.prototype.connect = function(name, query){
debug('connecting to namespace %s', name);
var nsp = this.server.nsps[name];
if (!nsp) {
  this.packet({ type: parser.ERROR, nsp: name, data : 'Invalid namespace'});
  return;
}

if ('/' != name && !this.nsps['/']) {
  this.connectBuffer.push(name);
  return;
}
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.run"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>run (event, fn)](#apidoc.element.socket.io.socket.prototype.run)
- description and source-code
```javascript
run = function (event, fn){
  var fns = this.fns.slice(0);
  if (!fns.length) return fn(null);

  function run(i){
    fns[i](event, function(err){
      // upon error, short-circuit
      if (err) return fn(err);

      // if no middleware left, summon callback
      if (!fns[i + 1]) return fn(null);

      // go on to next
      run(i + 1);
    });
  }

  run(0);
}
```
- example usage
```shell
...
 * @api private
 */

Namespace.prototype.add = function(client, query, fn){
  debug('adding socket to nsp %s', this.name);
  var socket = new Socket(this, client, query);
  var self = this;
  this.run(socket, function(err){
    process.nextTick(function(){
      if ('open' == client.conn.readyState) {
if (err) return socket.error(err.data || err.message);

// track socket
self.sockets[socket.id] = socket;
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.send"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>send ()](#apidoc.element.socket.io.socket.prototype.send)
- description and source-code
```javascript
send = function (){
  var args = Array.prototype.slice.call(arguments);
  args.unshift('message');
  this.emit.apply(this, args);
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.socket.io.socket.prototype.to"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>to (name)](#apidoc.element.socket.io.socket.prototype.to)
- description and source-code
```javascript
to = function (name){
  this._rooms = this._rooms || [];
  if (!~this._rooms.indexOf(name)) this._rooms.push(name);
  return this;
}
```
- example usage
```shell
...
only be _broadcasted_ to clients that have joined the given 'room'.

To emit to multiple rooms, you can call 'to' several times.

'''js
var io = require('socket.io')();
io.on('connection', function(client){
  client.to('others').emit('an event', { some: 'data' });
});
'''

### Socket#in(room:String):Socket

Same as 'Socket#to'
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.use"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>use (fn)](#apidoc.element.socket.io.socket.prototype.use)
- description and source-code
```javascript
use = function (fn){
  this.fns.push(fn);
  return this;
}
```
- example usage
```shell
...
Registers a middleware, which is a function that gets executed for
every incoming 'Socket', and receives as parameters the socket and a
function to optionally defer execution to the next registered
middleware.

'''js
var io = require('socket.io')();
io.use(function(socket, next){
  if (socket.request.headers.cookie) return next();
  next(new Error('Authentication error'));
});
'''

Errors passed to middleware callbacks are sent as special 'error'
packets to clients.
...
```

#### <a name="apidoc.element.socket.io.socket.prototype.write"></a>[function <span class="apidocSignatureSpan">socket.io.socket.prototype.</span>write ()](#apidoc.element.socket.io.socket.prototype.write)
- description and source-code
```javascript
write = function (){
  var args = Array.prototype.slice.call(arguments);
  args.unshift('message');
  this.emit.apply(this, args);
  return this;
}
```
- example usage
```shell
...
opts = opts || {};
var self = this;

// this writes to the actual connection
function writeToEngine(encodedPackets) {
  if (opts.volatile && !self.conn.transport.writable) return;
  for (var i = 0; i < encodedPackets.length; i++) {
    self.conn.write(encodedPackets[i], { compress: opts.compress });
  }
}

if ('open' == this.conn.readyState) {
  debug('writing packet %j', packet);
  if (!opts.preEncoded) { // not broadcasting, need to encode
    this.encoder.encode(packet, function (encodedPackets) { // encode, then write results to engine
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
