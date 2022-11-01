# NodeJs-preparation-Day-02
NodeJs-preparation-Day-02

<h2>Q.1 : What are the different types of HTTP requests?</h2>
HTTP (Hypertext Transfer Protocol) specifies a collection of request methods to specify what action is to be performed
on a particular resource.<br>
The most commonly used HTTP request methods are GET, POST, PUT, PATCH, and DELETE. These are equivalent to the CRUD
operations (create, read, update, and delete).
<ul>
    <li>GET : GET request is used to read/retrieve data from a web server. GET returns an HTTP status code of 200 (OK)
        if
        the data is successfully retrieved from the server.</li>
    <li>POST : POST request is used to send data (file, form data, etc.) to the server. On successful creation, it
        returns an HTTP status code of 201.</li>
    <li>PUT : A PUT request is used to modify the data on the server. It replaces the entire content at a particular
        location with data that is passed in the body payload. <br> If there are no resources that match the request, it
        will
        generate one.</li>
    <li>PATCH : PATCH is similar to PUT request, but the only difference is, it modifies a part of the data. It will
        only
        replace the content that you want to update.</li>
    <li>DELETE : A DELETE request is used to delete the data on the server at a specified location.</li>
</ul>


<h2>Q.2 : Explain the concept of middleware in Node.js.</h2>
Express.js is a routing and Middleware framework for handling the different routing of the webpage and it works between
the request and response cycle. <br>
Middleware gets executed after the server receives the request and before the controller actions send the response.<br>
Middleware has the access to the request object, responses object, and next, it can process the request before the
server send a response. An Express-based application is a series of middleware function calls.<br>
<h3>Middleware Chaining:</h3>
Middleware can be chained from one to another, Hence creating a chain of functions that are executed in order.<br>
The last function sends the response back to the browser. So, before sending the response back to the browser the
different middleware processes the request.<br>
The next() function in the express is responsible for calling the next middleware function if there is one.<br>
app.get(path, (req, res, next) => {}, (req, res) => {})


<h2>Q.3 : Explain CORS</h2>
<h3>CORS :</h3>
(Cross-Origin Resource Sharing) is a mechanism by which data or any other resource of a site could be shared
intentionally to a third party website when there is a need.<br>
Generally, access to resources that are residing in a third party site is restricted by the browser clients for security
purposes.


<h2>Q.4 : What is Express. how it helps you to create a backend application</h2>
<h3>Express.js:</h3>
Express is a small framework that sits on top of Node.js’s web server functionality to simplify its APIs and add helpful
new features. <br>
It makes it easier to organize your application’s functionality with middleware and routing. It adds helpful utilities
to Node.js’s HTTP objects. It facilitates the rendering of dynamic HTTP objects.

<ul>
    <li> More features than Node.js</li>
    <li> It is used to build web-apps using approaches and principles of Node.js.</li>
    <li> Routing is provided.</li>
    <li> It requires less coding time.</li>
    <li> Uses middleware for the arrangement of functions systematically server-side.</li>
    <li> import by const express = require ("express")</li>
</ul>


<h2>Q.5 : Explain min 5 status codes gets used in Backend development</h2>
An HTTP status code is a message a website's server sends to the browser to indicate whether or not that request can be
fulfilled. Status codes specs are set by the W3C.<br>
Status codes are embedded in the HTTP header of a page to tell the browser the result of its request.
<ul>
    <li>102 PROCESSING</li>
    <li>200 OK</li>
    <li>400 BAD_REQUEST</li>
    <li>401 UNAUTHORIZED</li>
    <li>402 PAYMENT_REQUIRED</li>
    <li>403 FORBIDDEN </li>
    <li>404 NOT_FOUND</li>
    <li>500 INTERNAL_SERVER_ERROR </li>
    <li>503 - Service Unavailable</li>
</ul>


<h2>Q.6 : Difference between HTTP and HTTPS</h2>
<ul>
    <li> HTTP is considered to be insecure and HTTPS is secure</li>
    <li> In HTTP, Encryption is absent and Encryption is present in HTTPS as discussed above</li>
    <li> HTTP does not require any certificates and HTTPS needs SSL Certificates</li>
    <li> HTTP speed is faster than HTTPS and HTTPS speed is slower than HTTP</li>
    <li> HTTP does not improve search ranking while HTTPS improves search ranking.</li>
</ul>


<h2>Q.7 : What are JWT tokens?</h2>
A JSON web token(JWT) is JSON Object which is used to securely transfer information over the web(between two parties).
<br>
It can be used for an authentication system and can also be used for information exchange.The token is mainly composed
of header, payload, signature. These three parts are separated by dots(.).
<br><br><br>
