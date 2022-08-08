# Message Queues

### what the Chat Example (above) does? 

We are Building a basic Chat server which will send the message automaticly to the user.

### What proof of life are we getting on the backend from the above app?

a user connected

### What flag would you use if you want to send a message to everyone except for a certain emitting socket?

Using broadcast Flag.

```
io.on('connection', (socket) => {
  socket.broadcast.emit('hi');
});

```

### What is a room and how might a room be useful?

A room is an arbitrary channel that sockets can join and leave. It can be used to broadcast events to a subset of clients

### How do you join a room?

```
io.on("connection", (socket) => {
  socket.join("some room");
});
```

### how do you leave a room?

``` 
io.on("connection", socket => {
  socket.on("disconnecting", () => {
    console.log(socket.rooms); // the Set contains at least the socket ID
  });

  socket.on("disconnect", () => {
    // socket.rooms.size === 0
  });
});
```

## Namespaces

### What is a Namespace and what does it allow you to do?

so what if we need to send a message only to a certain user? we will use Namespcaes which will target to a certain user only.

## Discuss a possible use case for separate namespaces

As I mentioned before like if there's some message or information that wan't to be sent to specefic user