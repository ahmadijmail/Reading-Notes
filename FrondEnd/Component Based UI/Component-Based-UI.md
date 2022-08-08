# Reading: Component Based UI

## React JS

### What is the difference between an element and a React component?
 

Basically, a React component describes what you need to see on the screen. Not all that basically, a React element is a protest portrayal of some UI. 

A React component is a function or a class which alternatively acknowledges input and returns a React component (ordinarily by means of JSX which gets transpiled to a createElement invocation).

### What are some advantages of React’s component based architecture?

In Component Driven Development, the development process is in place, components once created can be easily used across as many modules as needed.


## Introducing JSX

### What is JSX and why do we use it?

 it is a syntax extension to JavaScript. 

 it helpful as a visual aid when working with UI inside the JavaScript code. It also allows React to show more useful error and warning messages.

 ### Describe the process of embedding JavaScript expressions in JSX.


n the example below, we declare a variable called name and then use it inside JSX by wrapping it in curly braces:

```
const name = 'Josh Perez';
const element = <h1>Hello, {name}</h1>;
```


You can put any valid JavaScript expression inside the curly braces in JSX. For example, 2 + 2, user.firstName, or formatName(user) are all valid JavaScript expressions.


### Is it safe to embed user input in JSX? 

It is safe to embed user input in JSX:

By default, React DOM escapes any values embedded in JSX before rendering them. Thus it ensures that you can never inject anything that’s not explicitly written in your application.


## Rendering elements

### Explain what a React Component is to a non-technical friend.

It's like the thing that handel the elemnts you see in the screen.

### Describe mutability and React Components, specifically, how is the UI updated?

With our knowledge so far, the only way to update the UI is to create a new element, and pass it to root.render().


### If changes are made to the UI, what does React update?

React Only Updates What’s Necessary


 





