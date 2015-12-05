# React-starter
an extended starter for learning React with the official tutorial 
## Why this repo
As you can see this [tutorial](http://facebook.github.io/react/docs/tutorial. html) in the [React official site](http://facebook.github.io/react/index.html),this tutorial shows you how to develop an simple application with React.js,That is cool.However, it is too simple to guide the readers to build a whole application from scratch.Now this repo can help you to achieve three goals and build the environment for learning React easily.

* start a simple server to load resource and do some stuff with backend.
* you can download external libraries such as `React.js` or `React-dom.js` via npm and compile them in your devices as you want.
* with a babelrc file based configuration, you just focus on bundling `.js` files without considering the presets of babel.you can write code with `jsx` and `ES20115`.
## How to do
* download this repo via zip or git
``` git clone https://github.com/myzhibie/React-starter.git ```
* enter into the root directory
``` cd react-test ```
``` npm install ```
* write some code in `src/helloword.js` 
``` javascript
   var React=require('react');
var ReactDOM=require('react-dom');
ReactDOM.render(
    <h1>hello,world</h1>,
    document.getElementById('example')
    );
```
* bundle the source code via `browerify`
```   browserify -t [ babelify ] "./src/helloworld.js" -o "./build/helloworld.js" ```
this command will bundle the source code you write with its dependencies and transform its `jsx` and `ES2015` synax to plain javascript.
* link the bundled script to the `build/index.html` like this
``` html
<script type="text/javascript"  src="helloworld.js">
```
* start a server
``` node server.js ```
* preview `index.html` in [localhost:3000](http://localhost:3000) 

##Next step
the next step you have to do is following [this tutorial](http://facebook.github.io/react/docs/tutorial. html) and  do the other work,enjoy your learning!
