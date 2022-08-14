# Using the Effect Hook

## What purpose does useEffect serve in a function component compared to its counterpart(s) in class components?

The Effect Hook lets you perform side effects in function components

## What does useEffect do?

By using this Hook, you tell React that your component needs to do something after render. 

## Why is useEffect called inside a component?

Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. 

## Effects with Cleanup

Earlier, we looked at how to express side effects that don’t require any cleanup. However, some effects do. For example, we might want to set up a subscription to some external data source. In that case, it is important to clean up so that we don’t introduce a memory leak! Let’s compare how we can do it with classes and with Hooks.



