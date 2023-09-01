# Understanding Asynchronous Code, and API's
01. What is the difference between `asynchronous` code and `synchronous` code?

  > Async is multi-thread, which means operations or programs can run in parallel. Sync is single-thread. Asynchronous programming is a technique that enables your program to start a potentially long-running task and still be able to be responsive to other events while that task runs, rather than having to wait until that task has finished. Once that task has finished, your program is presented with the result.

02. What is an event listener?

  > An event listener is a programming construct. Example from some of our work this week is this line from our Controller class to setup our listener:     AppState.on('items', _drawItems). We have an emitter in our template that "matches" this event listener. 
 

03. What does *REST* stand for, and in simple terms what does it mean??

  > REST stands for REpresentational State Transfer. It is an architecture that governs rules for an application or servcie to communicate with other applications. It allows developers to have a higher flexibility, its more lightweight. RESTful API is called, the server will transfer to the client a representation of the state of the requested resource.


04. What is a callback / higher order function?

  > Callbacks are just the name of a convention for using JavaScript functions. There isn’t a special thing called a ‘callback’ in the JavaScript language, it’s just a convention. Instead of immediately returning some result like most functions, functions that use callbacks take some time to produce a result. The word ‘asynchronous’, aka ‘async’ just means ‘takes some time’ or ‘happens in the future, not right now’. Usually callbacks are only used when doing I/O, e.g. downloading things, reading files, talking to databases, etc.


05. What is a `promise`? How do you capture an error from a `promise`?

  > Promises are a way to write async code that still appears as though it is executing in a top-down way, and handles more types of errors due to encouraged use of try/catch style error handling.

06. Name three processes used to make requests over `HTTP`?

  > CRUD
  C - create
  R - read
  U - update
  D - delete

07. What does the `API` acronym stand for?

  > Application Programming Interface


08. What must you do in order to `await` a promise inside of a function?

  >In order to await a promise inside of a function, you need to mark the function itself as async.

09. What is the purpose of encapsulation in programming?

  > It protects against unwanted acccess to data.

10. What is `HTTP` response code for a successful request?

  > 200

11. What is a 400 error?

  > Description
The HTTP 400 Bad Request response status code indicates that the server cannot or will not process the request due to something that is perceived to be a client error (for example, malformed request syntax, invalid request message framing, or deceptive request routing).

Warning: The client should not repeat this request without modification.
See Also
Spec
Source: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status/400
