# Introducing Node

Defnition of Node (**Node.js**): runtime environment that allows developers to create all kinds of server-side tools and applications in JavaScript.<br>

## Frameworks: <br> 

Defnition of **Frameworks**: Are software that are developed and used by developers to build applications. <br> 

Benifet of using Frameworks:  <br> 
Make life easier for developers by allowing them to take control of the entire software development process, or most of it, from a single platform. <br> 

## Express: <br>

Defnition of **Express**: the most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks. <br> 

## middleware: <br>
It's used extensively in Express apps, for tasks from serving static files to error handling, to compressing HTTP responses.

## Handling errors:  <br>

we can handel errors using Midlleware functions.<br> 
Example:<br> 
```app.use(function(err, req, res, next) { ``` <br> 
 ``` console.error(err.stack);``` <br> 
 ``` res.status(500).send('Something broke!');``` 
```});``` <br> 

How to use Node and Express: we need to create web server using Node HTTP Package.<br> 
Steps: <br>

1- Making Server.js File : <br> 


const express = require('express'); <br>
const app = express(); <br>
const port = 3000;  <br>

app.get('/', function(req, res) {
  res.send('Ahmad Ijmail')
});

app.listen(port, function() {
  console.log(`Example app listening on port ${port}!`)
});

2- Run the serveru using ```node Server.js``` or ```nodemon```


## npm

Defnition of **npm**: it's a package manager for the JavaScript programming language maintained by npm, Inc. npm is the default package manager for the JavaScript runtime environment Node.js.  <br> 

## TDD

Defnition of **Test-driven development”**: It's the way that the code has been programed by which has 3 activities 
coding, testing, design.  <br> 

## CI/CD
Defnition of **Test-driven development”**: As we know in most cases any project need multiple people to work on it
so it need to be orgizned so you don't face errors like mergecomflict and other things, we have 2 options to do that. <br>
1- CI "**Continuous Integration**": it will help you ensure everyone's changes integrate, reduce merge conflicts, catch bugs.<br>

 ## 2- CD 
--2.1 **Continuous Delivery**: Develop to release at any time <br>
--2.2 **Continuous Deployment**: Deploy new features immediately<br>





