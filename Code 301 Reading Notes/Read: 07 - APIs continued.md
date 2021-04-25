## APIs

### REST

The whole world wide web is built on an architectural style called “REST”. REST provides a definition of a “resource”, which is what those things point to.

### SuperAgent

SuperAgent is light-weight progressive ajax API crafted for flexibility, readability, and a low learning curve after being frustrated with many of the existing request APIs. It also works with Node.js!

```
request
   .post('/api/pet')
   .send({ name: 'Manny', species: 'cat' })
   .set('X-API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(res => {
      alert('yay got ' + JSON.stringify(res.body));
   });
```

1. Request basics

```
request
   .get('/search')
   .then(res => {
      // res.body, res.headers, res.status
   })
   .catch(err => {
      // err.message, err.response
   });
```

- HTTP method may also be passed as a string: `request('GET', '/search').then(success, failure);`

- The Node client supports making requests to Unix Domain Sockets:

```
// pattern: https?+unix://SOCKET_PATH/REQUEST_PATH
//          Use `%2F` as `/` in SOCKET_PATH
try {
  const res = await request
    .get('http+unix://%2Fabsolute%2Fpath%2Fto%2Funix.sock/search');
  // res.body, res.headers, res.status
} catch(err) {
  // err.message, err.response
}
```

- DELETE, HEAD, PATCH, POST, and PUT requests can also be used

- DELETE can be also called as .del() for compatibility with old IE where delete is a reserved word.

2. Setting header fields

```
request
   .get('/search')
   .set('API-Key', 'foobar')
   .set('Accept', 'application/json')
   .then(callback);
```

3. GET requests. The .query() method accepts objects, which when used with the GET method will form a query-string.

4. HEAD requests

```
request
    .head('/users')
    .query({ email: 'joe@smith.com' })
    .then(res => {

    });
```

5. POST / PUT requests. A typical JSON POST request might look a little like the following, where we set the Content-Type header field appropriately, and "write" some data, in this case just a JSON string.

6. Response properties

- Response text
- Response body
- Response body
- Response Content-Type
- Response status

7. Error handling. Your callback function will always be passed two arguments: error and response. If no error occurred, the first argument will be null:

```
request
 .post('/upload')
 .attach('image', 'path/to/tobi.png')
 .then(res => {

 });
```
