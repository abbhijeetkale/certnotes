Node embraces non-blocking I/O to improve performance for a number of application types.

JavaScript’s traditional event-based implementation makes a relatively convenient
and well-understood syntax that suits asynchronous programming.

Node.js is a server-side framework, one of it’s main works is to handle any number of requests.
In traditional I/O bound servers systems, a request can only be issued when the response
to the previous request has arrived. This is typically referred to as blocking I/O.

Node.JS is a non-blocking I/O,
If a request takes long time, Node.js sends that request in an event loop
and moves on to handle the next request in the call stack.
As soon as the pending request is done processing, it raises an event and the
response is rendered on the browser.

Asynchronous Callbacks
In commonly in event driven architecture systems,
servers perform tasks that might take a while to complete,
like call an API or access a database. Node can process more incoming requests,
allowing you to handle thousands of concurrent connections with very little overhead,
as opposed to needing a thread on the server for each connection.