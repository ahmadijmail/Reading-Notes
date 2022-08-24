# Context API - Behaviors

## Necessity for the Design System

## Dream State

Render props and higher order components. We don’t want to deal with a messy React tree and wrappers. We don’t want action creators, reducers*, or any of that stuff.

## Globally Accessible


The state of our snackbars (which ones are visible) can be localized to a single centralized component. That same centralized component can be responsible for rendering them. There’s really no need for another component somewhere in the tree to hook into that state (at least not in our use-case).

## Higher Level API & Behaviour

There’s a lot more happening now. Our provider now exposes a new function called addAlert. This function uses the local state mutator useState to properly append a new alert without destroying existing ones.

## With regard to the React Context API, how would we implement a “consumer” role?

The other half of the puzzle is we now need a consumer for this provider. It turns out that our custom hook from before is nothing more than a small wrapper around the useContext internal React hook, which consumes our new context.



The other half of the puzzle is we now need a consumer for this provider. It turns out that our custom hook from before is nothing more than a small wrapper around the useContext internal React hook, which consumes our new context.

## Awesome React Context links

1. [Takeaway 1](https://github.com/jamiebuilds/create-react-context )
2.  [Takeaway 2](https://github.com/bowheart/react-zedux)
