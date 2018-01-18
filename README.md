# ReactStructure Startup

Use #create-react-app, lets create our new React single page application.

create-react-app react-redux-client

First of all we need to set up the redux and client side routing for our web application. Let’s install the dependencies.

npm install redux react-redux redux-thunk react-router@^3.0.0 react-router-redux react-bootstrap react-router-bootstrap@rr-v3 --save

redux is a library that helps you manage your app’s state. React bindings are not included in Redux by default. You need to install react-redux to use redux with react.js. redux-thunk middleware allows you to write action creators that return a function instead of an action. The thunk can be used to delay the dispatch of an action, or to dispatch only if a certain condition is met. react-router is a router library for react, it connects nicely to react and redux to help your app support routes. react-router-redux library helps you keep that bit of state in sync with your Redux store.

Lets do a bit of cleanup of unnecessary files to start.

cd src && rm App.test.js App.css favicon.ico index.css

Now create some new folders in the src directory.

mkdir actions components containers reducers store

To explain the different parts:
