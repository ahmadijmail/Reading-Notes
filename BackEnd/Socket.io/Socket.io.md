# Socket.io


## What is a Web Socket?

WebSocket is a computer communications protocol, providing full-duplex communication channels over a single TCP connection. 

![WebSocket](https://assets.stanko.io/blog/production/store/a6bad9b68057b2ed9716dd35ced216fa.gif)
## what happens once the connection is established ?

A real-time data transfer from and to the server. 

Web Sockets provide a standardized way for the server to send content to a client without first receiving a request from that client.


## What does the event handler io.on() do?

Start listening for socket events from Sails with the specified eventName.

Enables real-time bidirectional event-based communication. It works on every platform, browser or device, focusing equally on reliability and speed. 

## What does socket.emit() do?

send a message to all the connected clients.

## Real-time Applications
1. Instant messengers 
2. Push Notifications
3. Collaboration Applications
4. Online Gaming

## Socket.io vs Web Sockets

It's like JavasScript and react, they are 2 deffernt things, Socket.io is a library that uses web sockets connetionn, and Web Socket it's provied a bidirectional communication between the Client and the Server over a TCP connection; WebSocket remains open all the time, so they allow real-time data transfer.

## When would you use Socket.IO?

When you built real time applications, like Group chat Room, video conferencing, multiplayer games etc.

If you want server to push data by itself without calling from client.


## When would you use WebSockets?


When you built real time applications, like Group chat Room, video conferencing, multiplayer games etc.

If you want server to push data by itself without calling from client.