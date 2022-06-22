# Event-Driven Programming in Node.js

# EventEmitter

It allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challange, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.

We access the EventEmitter class through the events module. Once imported we’ll need to create a new object from the class to start using it.

js```const EventEmitter = require('events').EventEmitter;
const myEventEmitter = new EventEmitter;```


## A function that will act as our event listener, then we can use EventEmitters on method to set the listener.

```const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter;

function userJoined(username){
  // Assuming we already have a function to alert all users.
  alertAllUsers('User ' + username + ' has joined the chat.');
}

// Run the userJoined function when a 'userJoined' event is triggered.
chatRoomEvents.on('userJoined', userJoined); 
```

## Removing Listeners

To remove event listeners in EventEmitter we can use the removeListener or removeAllListeners method.

```
const EventEmitter = require('events').EventEmitter;
const chatRoomEvents = new EventEmitter;

function userJoined(username){
  chatRoomEvents.on('message', function(message){
    document.write(message);
  })
}

chatRoomEvents.on('userJoined', userJoined);
```
## Object Oriented Programming + Event-Driven Programming


```
Imagine we’re building a mail application. We might have an object whose sole purpose is to process the incoming and outgoing mail messages for our client. This object would contain all of its own behavioral functions. We might have a sendMail function that delivers our mail to a server. We might also have a receiveMail function that tells the server to deliver us any new mail it has for us. We’ll call the object responsible for these server interactions our Mailbox.
```