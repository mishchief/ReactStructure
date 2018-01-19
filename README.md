# ReactStructure Startup Manual

Use **create-react-app**, to create a new React single page application.

> create-react-app react-redux-client

Then set up the **redux** and client side routing for our web application. 

Dependencies:

> npm install redux react-redux redux-thunk react-router@^3.0.0 react-router-redux react-bootstrap react-router-bootstrap@rr-v3 --save

**redux** is a library that helps you manage your app’s state. React bindings are not included in Redux by default. You need to install **react-redux** to use redux with react.js. **redux-thunk** middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. **react-router** is a router library for react, it connects nicely to react and redux to help your app support routes. **react-router-redux** library helps you keep that bit of state in sync with your Redux store.

We then proceed to create some new folders in the src directory.

> cd src && mkdir actions components containers reducers store

To explain folder structure:

**Actions:** plain JavaScript objects that send data from your application to your store.
**Components:** let you split the UI into independent, reusable pieces, and think about each piece in isolation.
**Container:** component is a component that is responsible for retrieving data, and in order to get that data, the component needs to use Redux’s connect and mapStateToProps functions.
**Reducers:** are used to update the state object in your store. Just like actions, your application can have multiple reducers.
**Store:** is where the whole state tree of your application is based. The only way to change the state inside it is to dispatch an action on it. A store is not a class. It’s just an object with a few methods on it. To create it, pass your root reducing function to createStore.
