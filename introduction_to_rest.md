# Introducing REST

- REST stands for Representational State Transfer.
- REST is a set of Architectural Constraints.

## What are Resources?

- Resources are key abstractions in REST and represent any piece of information that can be named.
- Resources are entities or objects held by the server that can be accessed and manipulated by clients.
- Clients request resources via URLs.
- Servers respond with a representation of the resources to the client.

## What is Representational?

- The server returns a representation of the resource, not the actual resource.
- Representations can be in various formats like JSON, XML, HTML, etc.

## What is State of a resource? How REST is stateless?

- The state refers to the current condition of a resource at a particular point in time.
- REST is stateless, meaning each request from the client contains all the information needed by the server to fulfill that request.

## What is Transfer?

- Transfer refers to the act of moving the state of the representation of the resource between the client and server.
- This transfer happens over standard HTTP methods such as GET, POST, PUT, DELETE, etc.

## Introduction to HTTP protocol

### REST and Nouns

- In REST, nouns are used to represent resources.
- Resources are typically represented by URLs, which identify the resource. 
- Example: /products, /users, /orders.

### HTTP Methods

- HTTP methods such as GET, POST, PUT, DELETE, etc., define the action to be performed on the resources (nouns).
- These methods provide a standard way to interact with resources.

### Example

- HTTP method: GET
- Noun: Product
- Action: Retrieve all products.
- Example request: GET /products
- Example response: A list of all products available on the server.

---
# Need for Rest API

1. **Standardization**: REST uses standard methods (e.g., `GET /products`) for consistent resource interaction.
2. **Scalability**: Being stateless, REST allows servers to handle multiple requests independently, aiding scalability.
3. **Interoperability**: Standard HTTP methods enable different systems (e.g., mobile and web apps) to use the same API.
4. **Simplicity**: REST's use of standard HTTP protocols and methods makes it easy to understand and use.
5. **Flexibility**: REST supports multiple data formats (e.g., JSON, XML), making it adaptable for various client needs.

---
# What is API?
An API (Application Programming Interface) is a set of rules and tools that allows software applications to communicate with each other. It defines the methods and data formats that applications can use to request and exchange information.

In simple terms:
- **Interface**: It acts like a bridge between different software programs, enabling them to talk to each other.
- **Functionality**: APIs allow developers to use predefined functions to interact with an application or service without needing to understand its internal workings.
- **Example**: A weather app on your phone uses an API to fetch weather data from a remote server.

---
# What is Rest API?
A REST API (Representational State Transfer Application Programming Interface) is a type of API that adheres to the principles of REST. It allows different software applications to communicate over the web using standard HTTP methods. Here's a simple breakdown:

1. **Resource-Based**: REST APIs manage resources, which are identified using URLs (e.g., `/users`, `/products`).

2. **HTTP Methods**: They use standard HTTP methods to perform operations on resources:
    - **GET**: Retrieve a resource.
    - **POST**: Create a new resource.
    - **PUT**: Update an existing resource.
    - **DELETE**: Remove a resource.

3. **Stateless**: Each request from a client to a server must contain all the information needed to understand and process the request. The server does not store any client context between requests.

4. **Representations**: Resources are represented in standard formats like JSON or XML, which are transferred between the client and server.

5. **Uniform Interface**: A consistent and predictable way to access and manipulate resources.

---
# What is Web API?

1. **Web API Definition**: Facilitates communication between applications over the web, allowing access to external functionalities or data.
2. **Example Scenario**: A product website integrates Google Maps API for location services and Amazon API for seamless online ordering.
3. **Functionality Enhancement**: APIs enhance user experience by integrating interactive maps and e-commerce capabilities directly into the website.
4. **Integration Benefits**: Leveraging external APIs (Google Maps, Amazon) enriches website functionality without needing to build these services from scratch.
5. **Overall Impact**: APIs streamline development, improve user interaction, and expand service offerings by integrating with established platforms like Google and Amazon.

---
# A comparison of APIs

| Concept      | Definition                                                                   | Example                                                         |
|--------------|------------------------------------------------------------------------------|-----------------------------------------------------------------|
| Web API      | General term for any API exposed over the web, enabling system interaction.  | Twitter API for interacting with tweets.                        |
| REST API     | Uses REST architectural style with standard HTTP methods (GET, POST, etc.).  | GitHub API for managing repositories.                           |
| Web Service  | Supports interoperable machine-to-machine interaction over a network.        | AWS services like Lambda for serverless computing.              |
| SOAP         | Protocol for exchanging structured information in web services.              | Financial transactions using SOAP for security and reliability. |

---
