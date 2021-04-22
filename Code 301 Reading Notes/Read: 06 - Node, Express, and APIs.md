## What Is Node and When Should I Use I

- Node.js® is a JavaScript runtime built on Chrome’s V8 JavaScript engine.
- Node.js is an event-based, non-blocking, asynchronous I/O runtime that uses Google’s V8 JavaScript engine and libuv library.

### Node Is Built on Google Chrome’s V8 JavaScript Engine

The V8 engine is the open-source JavaScript engine that runs in Google Chrome and other Chromium-based web browsers, including Brave, Opera, and Vivaldi.

### Node Binaries vs Version Manager

Many websites will recommend that you head to the official Node download page and grab the Node binaries for your system. While that works, I would suggest that you use a version manager instead. This is a program that allows you to install multiple versions of Node and switch between them at will.

### “Hello, World!” the Node.js Way

check that Node is installed `node -v`

create a new file `hello.js` and copy in the following code: `console.log("Hello, World!");`

run `node hello.js`

### npm - package manager

check version `npm -v`

### Installing a Package Globally

`npm install -g jshint`

### Installing a Package Locally

`npm init -y`
`npm install lodash --save`

test.js

```
const _ = require('lodash');

const arr = [0, 1, false, 2, '', 3];
console.log(_.compact(arr));
```

### What Is Node.js Used For?

Designed to automate the process of developing a modern JavaScript application.

### “Hello, World!” — Server Version

```
const http = require('http');

http.createServer((request, response) => {
  response.writeHead(200);
  response.end('Hello, World!');
}).listen(3000);

console.log('Server running on http://localhost:3000');
```

### What Are the Advantages of Node.js?

1. using JavaScript on a web server — as well as in the browser
2. it speaks JSON. JSON is probably the most important data exchange format on the Web, and the lingua franca for interacting with object databases (such as MongoDB)
3. transitioning to Node development is potentially easier than to other server-side languages
