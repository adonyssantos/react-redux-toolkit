# Global State Management with Redux

## What is redux?

Redux is a predictable state container for JavaScript applications. It is often used with React, but it can be used with any other UI library or framework.

The core concept of Redux is to store the entire state of an application in a single, centralized store. The state is updated by dispatching actions, which are plain JavaScript objects that describe what should change in the state. A reducer function then takes the current state and the action, and returns a new state object that reflects the changes described in the action.

Redux also provides a set of utilities for managing asynchronous actions, such as middleware and thunks. Middleware allows for additional processing of actions before they reach the reducers, while thunks are functions that can dispatch multiple actions and interact with the store asynchronously.

By keeping the state of an application in a single, predictable location, Redux simplifies the process of tracking changes and debugging problems in a complex application. It also encourages a more functional programming style by making it easier to reason about the flow of data through an application.

## What is a state manager?

A state manager is a tool that manages the state application.

In a React-Redux application, components are typically divided into two types: \

1. **Presentational components:** are responsible for rendering the UI
2. **Container components:** are responsible for managing the state of the application.

**Container components** subscribe to the Redux store and pass the state down to the presentational components as props. When the state changes, the container components update the state in the store, which triggers a re-render of the **presentational components**.

Redux also provides a way to **dispatch actions** to update the state of the application. Actions are plain JavaScript objects that describe what should change in the state, and **reducers** are functions that take the current state and an action and return a new state object that reflects the changes described in the action.

By using Redux as a state manager in a React application, developers can more easily manage the state of the application and ensure that updates to the state are consistent and predictable. This can lead to more maintainable and bug-free code over time.
