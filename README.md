Socket.js minimal starter kit for Windows Azure
===========

1. Fork this repo and connect with your Azure to deploy. When the repo is pushed to Github, It will be automatically deployed to Azure with `npm install`.
2. Turn on WebSocket [ CONFIGURE > WEB SOCKETS ], and then restart the server. That's it on Azure side!
3. For client page, open **_client/index.html** and replace following 2 lines containing `***` for your Azure project.

```
<script src="http://***.azurewebsites.net/socket.io/socket.io.js"></script>
```

and

```
var socket = io.connect( 'http://***.azurewebsites.net' );
```

4.  Launch a local server or host it on a www server, as _client dir for root.

Then you will see a simple chat running with socket.io on Azure!
