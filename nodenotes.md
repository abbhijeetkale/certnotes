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

https://dzone.com/articles/design-patterns-in-expressjs

Monkey Patch
Hooks



Further reading : https://code.tutsplus.com/articles/mapping-relational-databases-and-sql-to-mongodb--net-35650
Developers can develop application which can be agnostic about deployments. MongoDB supports scaling out as opposed to RDBMS which supports scaling up. 

node.js is basically a C++ program that you control using V8 javascript. So any applications you write using node.js will be written in javascript and it will control this C++ application (node.js) and you’ll be able to say something like they made request for this resource and your application actually in javascript will say: okey, they made a request for this resource, I don’t have to respond to that. Now respond accordingly.

https://hackernoon.com/mongodb-for-node-js-developers-jumpstart-a1520182850e

Node.js connects to MongoDB using drivers. Installing 32 bit release shall be avoided because it limits the addressable size of data using the default storage engine.

https://www.codementor.io/codementorteam/nodejs-profiling-build-a-high-performance-app-babjg4jf9

https://www.rainforestqa.com/blog/2012-11-05-mongodb-gotchas-and-how-to-avoid-them/
https://www.blazemeter.com/blog/how-load-test-mongodb-jmeter

https://docs.mlab.com/troubleshooting-connection-issues/

https://stackoverflow.com/questions/44422797/mongoose-connect-throwing-a-warning

https://medium.com/createdd-notes/starting-with-authentication-a-tutorial-with-node-js-and-mongodb-25d524ca0359

https://dzone.com/articles/leverage-http-status-codes-to-build-a-rest-service
https://benramsey.com/blog/2008/05/http-status-204-no-content-and-205-reset-content/
https://stackoverflow.com/questions/11746894/what-is-the-proper-rest-response-code-for-a-valid-request-but-an-empty-data


https://medium.com/@augusteo/easy-functional-and-integration-testing-with-mock-server-tutorial-and-example-c338d33f971d

http://tech.namshi.io/blog/2014/06/13/mockserver-effortless-api-mocking-library-in-node-js/

https://www.npmjs.com/package/mockserver

https://github.com/CyberAgent/node-easymock

https://coderwall.com/p/ss80vw/using-node-js-with-express-as-a-simple-api-mock-server

https://forum.raml.org/t/raml-1-0-to-rest-json-client-converter/2195

https://github.com/raml-org/raml-spec/issues/618

https://github.com/raml-org/ramldt2jsonschema

https://codebeautify.org/yaml-to-json-xml-csv/cb83e104


https://hackernoon.com/mongodb-schema-design-86327d8fae83

https://dev.to/mrm8488/mongodb-schema-design-patterns-i-4gdp

https://cs.nyu.edu/courses/Fall12/CSCI-GA.2433-001/
http://www.ccs.neu.edu/home/kathleen/classes/cs3200/20-NoSQLMongoDB.pdf

https://github.com/AntonioErdeljac/file-upload-tutorial.git


https://azure.microsoft.com/en-in/resources/samples/storage-blob-upload-from-webapp-node/ : this looks good to me

https://www.diycode.cc/projects/Azure/azure-storage-node

https://azure.microsoft.com/en-in/resources/samples/storage-blob-upload-from-webapp-node/

https://stackoverflow.com/questions/13546249/authorization-approaches-and-design-patterns-for-node-js-applications
https://www.npmjs.com/package/node-authorization
https://hashnode.com/post/authorization-solution-for-nodejs-ciibz8fo401ffj3xt3vhle6eb
https://blog.nodeswat.com/implement-access-control-in-node-js-8567e7b484d1

https://fourminutebooks.com/the-black-swan-summary/
https://www.stat.berkeley.edu/~aldous/157/Books/taleb.html


http://www.componentix.com/blog/9/file-uploads-using-nodejs-now-for-real


https://grokonez.com/node-js/nodejs-save-file-image-to-mysql-by-sequelize-with-blob-type

https://philna.sh/blog/2016/06/13/the-surprise-multipart-form-data/


https://photograph.blob.core.windows.net/competencyimages/offer-default.jpg

https://github.com/kadirahq/mongo-mask/blob/master/README.md#start-of-content

https://www.kenwalger.com/blog/nosql/mongodb/importing-data-mongoimport/

https://github.com/typicode/json-server

https://github.com/CyberAgent/node-easymock

https://github.com/namshi/mockserver/tree/master/test/mocks

https://www.npmjs.com/package/node-mock-server

https://itnext.io/how-to-mock-dependency-in-a-node-js-and-why-2ad4386f6587

https://medium.freecodecamp.org/how-to-mock-requests-for-unit-testing-in-node-bb5d7865814a

https://github.com/NaturalHistoryMuseum/ke2mongo/blob/master/ke2mongo/tasks/dataset.py

https://coderwall.com/p/ss80vw/using-node-js-with-express-as-a-simple-api-mock-server

https://www.akadia.com/services/sendmail_relay.html : SMTP relay

https://codeburst.io/grouping-array-data-json-ef96b438b927

https://stackoverflow.com/questions/15938859/mongodb-aggregate-within-daily-grouping

https://www.compose.com/articles/aggregations-in-mongodb-by-example/

http://www.kamsky.org/stupid-tricks-with-mongodb/more-fun-with-dates-and-aggregations

https://www.loggly.com/ultimate-guide/node-logging-basics/

https://www.digitalocean.com/community/tutorials/how-to-use-winston-to-log-node-js-applications

https://blog.exploratory.io/an-introduction-to-mongodb-query-for-beginners-bd463319aa4c

https://github.com/ctstone/winston-azure-storage-transport
