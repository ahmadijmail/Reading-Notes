# Context API

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

### Why might we use Context?

In a typical React application, data is passed top-down (parent to child) via props, but such usage can be cumbersome for certain types of props (e.g. locale preference, UI theme) that are required by many components within an application. Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

### Why should we use it sparingly?

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. 


1. Take away :

https://github.com/jamiebuilds/create-react-context

2. Take away :

https://github.com/drcmda/react-contextual