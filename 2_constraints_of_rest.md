# Constraints of REST
- Client-Server
- Stateless
- Cache
- Uniform Interface
- Layered System
- Code on Demand

## Client-Server
- This constraints states that a REST application should have a Client Server architecture.
- Advantage is Client and Server are separated.
- They can evolve independently.
- Client need not know anything about business logic/data access layer.
- Server need not know anything about the frontend UI
- Example: Web browsers (clients) interacting with various websites (servers) for browsing, shopping, or streaming.

## Stateless
- Stateless constraints states that server does not store any session data.
- However, client can save session data.
- The communication between the client and server is stateless.
- It means that all the information to understand a request is contained within the request.
- Improves Scalability.
- Example: HTTP, where each request from a browser to a server contains all necessary information (like cookies or tokens) for processing.

## Cache
- Cache constraint states responses should be cacheable, if possible.
- It required that every response should include whether a response can be cacheable or not.
- For subsequent request, the Client can retrieve form its cache, no need to send request to the Server asking data which is already stored in cache. 
- Reduces network latency and improves performance.
- Example: Web browsers caching images, scripts, or stylesheets to speed up page load times.

## Uniform Interface
- Uniform interface is the key differentiator between REST and Non-REST APIs.
- We have different devices and these devices use different software, the way of by which these devices interact with the server should be uniform.
- Defines the interface between clients and servers to promote simplicity and decoupling.
- There are 4 elements of Uniform Interface constraints.
  - **Resource Identification:** Resources (such as documents, images, or data) should be uniquely identified by URIs (Uniform Resource Identifiers). These URIs should provide a global addressing scheme for resources.
  - **Resource Manipulation through Representations:** Resources should be manipulated through representations, which are typically JSON or XML representations of the resource state. Clients interact with resources by exchanging representations of the resource state.
  - **Self-Descriptive Messages:** Each message sent between client and server should include enough information to describe how to process the message.
  - **Hypermedia as the Engine of Application State (HATEOAS):** The server should provide hypermedia links in the response dynamically to guide the client through the application state. This allows the server to evolve its API without breaking clients that understand previous versions.
- Example: RESTful APIs using HTTP methods (GET, POST, PUT, DELETE) and URIs (URLs) for resource manipulation, like Twitter API for tweets or GitHub API for repositories.

## Layered System
- According to the REST architectural style, a layered system means that the architecture is composed of hierarchical layers where each layer has a specific role and responsibility. 
- Clients interact with the outermost layer, typically a web server or an API gateway, which in turn may interact with other internal layers such as load balancers, caching servers, application servers, and databases.
- From the client's perspective, it communicates directly with a single server (the outermost layer), unaware of any intermediaries that may exist between it and the actual server processing its request.
- This transparency ensures that the client's interaction remains consistent regardless of the infrastructure changes made to improve performance, scalability, or security.
- In practice, a client might send a request to api.example.com, which could be served directly by a load balancer that distributes the request to one of several backend servers. These backend servers, in turn, may interact with databases or other services to fulfill the request. 
- The client remains unaware of the specific server handling its request or any intermediate steps taken to process it.

## Code on demand
- Optional constraint.
- In addition to data, the server can provide executable code to the client.
- This constraint is rarely used in modern RESTful architectures.
