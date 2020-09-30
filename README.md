## What is HTTP ? 🤔 

When it comes to HTTP, the first thought that comes to mind is about using
internet, is the scenario where we really see the use of HTTP in practice. We access
sites where their addresses start with http: // and so we need to know what really
is happening when doing this.
The moment you accessed this course, this class, between the browser and Alura happened
communication, and this communication has two well-known parts that we call
Client-Server or in Portuguese Client-Server. This is an architectural model, that is, the
The entire internet is based on this architecture where there is a client that requests and a server that responds.

*Client (Browser like Chrome or Firefox) -> Internet -> Server (Using PHP, JAVA or NET among others)*

In any communication, there must be some rules for the two parties to be able to
successfully understand. Thinking about your browser communication between Alura or some other
site this set of rules is basically a protocol, where in this scenario is HTTP.

Protocols are defined, specified and made available for implementation in
both parties, to consult the HTTP specification, you can use the following
address: https://tools.ietf.org/html/rfc2616

Client (Browser like Chrome or Firefox) -> Communication rules? -> Server (Using PHP, JAVA or NET among others)

#### Summing up:
*HTTP is a protocol that defines the rules of communication between client and server on the internet.*

#### Example:
*Client (Browser like Chrome or Firefox) -> HTTP (protocol) -> Server (Using PHP, JAVA or NET among others)*

## Modules

### 01. What is HTTP?

↪️ On the internet there is always a client and a server

↪️ There must be communication rules between the client and the server

↪️ Rules are defined within a protocol

↪️ HTTP is the most important protocol on the internet


### 02. The secure web - HTTPS

↪️ By default, data is trafficked as plain text on the web.

↪️ Only with HTTPS the web is secure

↪️ The HTTPS protocol is nothing more than the HTTP protocol plus an additional layer of security, TLS / SSL

↪️ The type of public key / private key encryption

↪️ What are digital certificates

↪️ Certificates have identity and validity

↪️ Public keys are in the certificate, the private key is only on the server

↪️ What is a certification authority

↪️ The browser uses the public key to encrypt the data


### 03. Addresses under your domain

↪️ URL is the web addresses

↪️ A URL begins with the protocol (for example https: //) followed by the domain (https://github.com)

↪️ After the domain can come the port, if not defined, the standard port of this protocol is used

↪️ After the domain: port, the path to a resource is specified (/devgabrieldejesus/http-basics)

↪️ A resource is something concrete in the application that we want to access


### 04. The client asks and the server answers

↪️ The HTTP protocol follows the Request-Response model

↪️ Always the customer initiates communication

↪️ A request must have all the information for the server to generate the response

↪️ HTTP is stateless, does not keep information between requests

↪️ Development platforms use sessions to store information between request


### 05. Debugging the HTPP request
↪️ Debug console

↪️ HTTP GET Method

↪️ Response header

↪️ Response codes (Status Code)


### 06. Request parameters

↪️ Used to define survey details or submit form data

↪️ GET: ss parameters are sent in the URL itself (using [?] And concatenating with [&])

↪️ POST: parameters are sent in the request body

↪️ HTTP️ There are other HTTP methods like POST, DELETE, PUT

#### Summary

↪️ GET: Receive data (Parameters in the URL)
 
↪️ POST: Submit data (Parameters in the request body)
 
↪️ DELETE: Remove a resource
 
↪️ PUT / PATCH: Update a resource


### 07. Web services with REST

↪️ REST is an architectural standard for communications between applications

↪️ It takes advantage of the HTTP structure

↪️ Resources are defined via URI

↪️ Operations with HTTP methods (GET / POST / PUT / DELETE)

↪️ Headers (Accept / Content-Type) are used to specify representations (JSON, XML, ...)

### 💡 To learn more: data types

In some HTTP headers we must specify some format. The formats are called in the MIME types documentation. And in the definition of the header we use the following structure: type / subtype. Known types are:

`text, image, application, audio and video`

And some subtypes:

`text -> text / plain, text / html, text / css, text / javascript`

`image -> image / gif, image / png, image / jpeg`

`audio -> audio / midi, audio / mpeg, audio / webm, audio / ogg, audio / wav`

`video -> video / mp4`

`application -> application / xml, application / pdf`

`Other formats accepted: https: // developer.mozilla.org / en-US / docs / Web / HTTP / Basics_of_HTTP / MIME_types`
