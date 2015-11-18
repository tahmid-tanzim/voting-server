# Voting Server

### 1. Project Setup
It's time to get our hands dirty. Before we do anything else, we need to create a project directory and initialize it as an NPM project:
```
mkdir voting-server
cd voting-server
npm init -y
```
This results in a directory with the single file `package.json` in it.

We're going to be writing our code in ES6. Altough Node supports many ES6 features starting at version 4.0.0, it still doesn't support modules, which we want to use. We'll need to add Babel to the project, so that we can use all the ES6 features we want and transpile the code to ES5:
```
npm install --save-dev babel-core babel-cli babel-preset-es2015
```
Since we'll be writing a bunch of unit tests, we'll also need some libraries to write them with:
```
npm install --save-dev mocha chai
```
One of the first libraries we're going to be using is Facebook's Immutable, which provides a number of data structures for us to use. We're going to start discussing Immutable in the next section, but for now let's just add it to the project, along with the chai-immutable library that extends Chai to add support for comparing Immutable data structures:
```
npm install --save immutable
npm install --save-dev chai-immutable
```
[Redux](http://redux.js.org/) is a predictable state container for JavaScript apps
```
npm install --save redux
```
Setting Up a [Socket.io](http://socket.io/) Server
```
npm install --save socket.io
```
### 2. Run the tests with the npm command
```
npm run test
```
