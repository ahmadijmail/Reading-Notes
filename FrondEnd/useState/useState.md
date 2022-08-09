# useState() Hook


## Introducing Hooks

### What was the motivation for introducing Hooks?

Hooks solve a wide variety of seemingly unconnected problems in React that we’ve encountered over five years of writing and maintaining tens of thousands of components.

### What changes are important regarding implementing Hooks versus Component Classes?

In addition to making code reuse and code organization more difficult, we’ve found that classes can be a large barrier to learning React. 
can understand props, state, and top-down data flow perfectly well but still struggle with classes. The distinction between function and class components in React and when to use each one leads to disagreements even between experienced React developers.

### Hooks allow you to reuse stateful logic without changing

Hooks let you use more of React’s features without classes. Conceptually, React components have always been closer to functions. Hooks embrace functions, but without sacrificing the practical spirit of React. Hooks provide access to imperative escape hatches and don’t require you to learn complex functional or reactive programming techniques.


## hooks api

### Name two rules imposed by React Hook usage

1. Only call Hooks at the top level. Don’t call Hooks inside loops, conditions, or nested functions.
2. Only call Hooks from React function components. Don’t call Hooks from regular JavaScript functions. (There is just one other valid place to call Hooks — your own custom Hooks. We’ll learn about them in a moment.)

## Using the State Hook

``` 
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

### What is a Hook?


Hooks are a new addition in React 16.8. They let you use state and other React features without writing a class.

### When would I use the useState Hook?


If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component. We’re going to do that right now!

### If you were to add React state to a function component by declaring a state variable:

1. What does calling useState do?

It declares a “state variable”.

2. What do we pass to useState as an argument?

The only argument to the useState() Hook is the initial state. Unlike with classes, the state doesn’t have to be an object. We can keep a number or a string if that’s all we need. In our example, we just want a number for how many times the user clicked, so pass 0 as initial state for our variable. (If we wanted to store two different values in state, we would call useState() twice.)

3. What does useState return?

 It returns a pair of values: the current state and a function that updates it. This is why we write const [count, setCount] = useState(). This is similar to this.state.count and this.setState in a class, except you get them in a pair.
