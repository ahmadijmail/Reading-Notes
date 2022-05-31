# Express REST API

# Classes
Defintion of **Classes**: Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are not shared with ES5 class-like semantics.<br>

## Dlass Declaration:  
we will use Class keyword with the name of the class. <br>
Example: <br>
class room {
  constructor(displacemnt, width) { <br>
    this.displacemnt = displacemnt; <br>
    this.width = width; <br>
  }
}

## Hoisting: ##  
The difference between function declarations and class declarations is that while functions can be called in code that appears before they are defined, classes must be defined before they can be constructed.<br>

## Class expressions: 
we can define class using expressions, it can be named or unamed.<br>

## Class body and method definitions:
1. Strict mode <br>
2. Constructor <br>
3. Static initialization blocks <br>
4. Prototype methods <br>
5. Generator methods <br>
6. Static methods and properties <br>


# Routing <br>

Defintion of **Routing**: it's how an application’s endpoints (URIs) respond to client requests. For an introduction to routing. <br>

Example: <br>
Get Method: <br>
```app.get('/', (req, res) => { ```
 ``` res.send('GET request to the homepage') ``` 
```})``` <br>
Post Method: <br>
```app.post('/', (req, res) => {```
 ``` res.send('POST request to the homepage')```
```})``` <br>

## Route paths <br> 

It's a mix between the request method and where exactly the method will be matched.

Example: localhost:3000/home <br>
```app.get('/home', (req, res) => {```
 ``` res.send('home')})```


## Route parameters <br>
They are named URL segments that are used to capture the values specified at their position in the URL. <br>

Example: <br>
```app.get('/users/:userId/books/:bookId', (req, res) => {```
 ``` res.send(req.params)}) ```

## Route handlers <br>
so when the user enter a speceifc path we need to send something to be shown, and that what route handlers do. 
```app.get('/example/a', (req, res) => {```
 ``` res.send('Hello from A!')})```

## ExpressJS <br>

How to use it: <br>

1. create server.js <br>
2. ```npm install``` <br>
3. In our server.js we need to setup the invromnt for the server to start, using the following: <br>

```js 


    const  express= require('express');
    const  app= express();
    const  port= process.env.PORT || 8080;

       
    app.get('/', function(req, res) {
        res.send('we Are in Home');
    });

    
    app.listen(port);
    console.log('Magic happens on port ' + port); 
   ```
## Route Middleware router.use(): 
In somecases we need to do something before the request like checking so we will need the **Route middleware**. 

   
    




