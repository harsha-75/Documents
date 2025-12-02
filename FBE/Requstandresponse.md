## REQUEST AND RESPONCE

### Request Responce Model

- client sends a request
- server parses the request
- server processes the request
- server sends the Response
- client parses the Responce and consume

### where it is Used ?

- HTTP, WEB, DNS,SSH
- RPC ( Remote Procedure Call)
- SQL and Database Protocols
- API (REST/SOAP/GraphQL)


### Anatomy of Request/Responce 

-  A request structure is defined by the both client and server
-  Request has a boundary
-  Defined by a protocal and message format


### EXAMPLE : Building an upload image service with request responce

- send a large request with the image (simple)
- chunck image and send a request per chunk (Resumable)


### Request Responce Model does not work for all cases some examples are here

 - Notification service
 - Chattng Application
 - Very Long Requests 
 - What if client disconnects ?
