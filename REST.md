
# REST




## 1. Introduction:
- REST stands for REpresentational State Transfer and API stands for Application Program Interface. REST is a software architectural style that defines the set of rules to be used for creating web services. Web services which follow the REST architectural style are known as RESTful web services. It allows requesting systems to access and manipulate web resources by using a uniform and predefined set of rules. Interaction in REST based systems happen through Internet’s Hypertext Transfer Protocol (HTTP). 

- A Restful system consists of a client who requests for the resources and server who has the resources.




![REST API](https://raw.githubusercontent.com/Codecademy/articles/0b631b51723fbb3cc652ef5f009082aa71916e63/images/rest_api.svg)





## 2. Why Use REST APIs:
- REST APIs are similar to SOAP in architectural terms.

- REST works on top of the HTTP transport. It takes advantage of HTTP’s native capabilities, such as GET, PUT, POST and DELETE. When a request is sent to a RESTful API, the response (the “representation” of the information “resource” being sought) returns in either the JSON, XML or HTML format. A RESTful API is defined by a web address, or Uniform Resource Identifier (URI), which typically follows a naming convention.

- In contrast to SOAP, REST is easier to work with and more flexible:

- No expensive tools needed in order for interaction with web services.
- Shorter learning curve.
- More efficient (XML, used in SOAP messages, is longer than REST’s message formats).
- Faster, with less processing required.

## 3. Architectural Constraints of RESTful API
- 3.1 Uniform Interface

- 3.2 Stateless

- 3.3 Cacheable

- 3.4 Client-Server

- 3.5 Layered System

- 3.6 Code on Demand





### 3.1 Uniform Interface:
- It is a key constraint that differentiate between a REST API and Non-REST API. It suggests that there should be an uniform way of interacting with a given server irrespective of device or type of application (website, mobile app). 

- There are four guidelines principle of Uniform Interface are:

- Resource-Based: Individual resources are identified in requests. For example: API/users.
- Manipulation of Resources Through Representations: Client has representation of resource and it contains enough information to modify or delete the resource on the server, provided it has permission to do so. Example: Usually user get a user id when user request for a list of users and then use that id to delete or modify that particular user.
- Self-descriptive Messages: Each message includes enough information to describe how to process the message so that server can easily analyses the request.



### 3.2 Statelessness:
- Systems that follow the REST paradigm are stateless, meaning that the server does not need to know anything about what state the client is in and vice versa. In this way, both the server and the client can understand any message received, even without seeing previous messages. This constraint of statelessness is enforced through the use of resources, rather than commands. Resources are the nouns of the Web - they describe any object, document, or thing that you may need to store or send to other services.

- Because REST systems interact through standard operations on resources, they do not rely on the implementation of interfaces.



### 3.3 Cacheable:
- Every response should include whether the response is cacheable or not and for how much duration responses can be cached at the client side. Client will return the data from its cache for any subsequent request and there would be no need to send the request again to the server. A well-managed caching partially or completely eliminates some client–server interactions, further improving availability and performance. But sometime there are chances that user may receive stale data. 


### 3.4 Client-Server:
- REST application should have a client-server architecture. A Client is someone who is requesting resources and are not concerned with data storage, which remains internal to each server, and server is someone who holds the resources and are not concerned with the user interface or user state. They can evolve independently. Client doesn’t need to know anything about business logic and server doesn’t need to know anything about frontend UI. 

### 3.5 Layered system:
- An application architecture needs to be composed of multiple layers. Each layer doesn’t know any thing about any layer other than that of immediate layer and there can be lot of intermediate servers between client and the end server. Intermediary servers may improve system availability by enabling load-balancing and by providing shared caches. 


### 3.6 Code on demand:
-  It is an optional feature. According to this, servers can also provide executable code to the client. The examples of code on demand may include the compiled components such as Java applets and client-side scripts such as JavaScript. 


## 4. Summary:
- In simple words, in the REST architectural style, data and functionality are considered resources and are accessed using Uniform Resource Identifiers (URIs).

- The resources are acted upon by using a set of simple, well-defined operations. Also, the resources have to be decoupled from their representation so that clients can access the content in various formats, such as HTML, XML, plain text, PDF, JPEG, JSON, and others.

- The clients and servers exchange representations of resources by using a standardized interface and protocol. Typically HTTP is the most used protocol, but REST does not mandate it.

- Metadata about the resource is made available and used to control caching, detect transmission errors, negotiate the appropriate representation format, and perform authentication or access control.

- And most importantly, every interaction with the server must be stateless.

- All these principles help RESTful applications to be simple, lightweight, and fast.



## Acknowledgements

 - [GeeksforGeeks](https://www.geeksforgeeks.org/rest-api-architectural-constraints/)
 - [akana](https://www.akana.com/blog/what-is-rest-api)
 - [codecademy](https://www.codecademy.com/article/what-is-rest)
 - [restfulapi](https://restfulapi.net/)

