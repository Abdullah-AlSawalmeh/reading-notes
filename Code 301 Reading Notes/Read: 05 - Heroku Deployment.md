# Heroku

## What is is used for?

- Heroku is a trusted container-based cloud Platform as a Service. Heroku lets you deploy, run and manage applications written in a lot of languages like Ruby, Node.js, Java, Python, Clojure, Scala, Go and PHP.

# Node.js For Beginners. Deploy Your Blog to Heroku

To see how servers work from within, we can build a simple web server by ourselves.

We use Node.js as a server part technology for that task.

- Node.js is an open source, a JS framework that lets you build back-end server side code with a cross-platform runtime environment.

First of all, we need to create a JavaScript file. Let's name it server.js:
var http = require("http");

http.createServer(function(request, response) {
response.writeHead(200, {"Content-Type": "text/plain"});
response.write("It's alive!");
response.end();
}).listen(3000);
It's a simple server and we can make sure it's running by typing (node server.js) in your terminal.
