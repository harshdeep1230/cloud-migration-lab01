# CST8915 Lab 1: Algonquin Pet Store on Azure VM

**Student Name**: Harshdeep puri
**Student ID**: 41170600
**Course**: CST8915 Full-stack Cloud-native Development
**Semester**: Winter 2026

---

## Demo Video

https://www.youtube.com/watch?v=S7gQ8vr3SKI
---

## Technical Explanations

### Order Service (Node.js)


The Order Service takes care of the complete life of a customer order including its creation as well as status tracking. It is written in Python and Flask, and relies on this stack due to its simplicity and the fact that it supports RESTful routing with the minimal amount of overhead. It utilizes a separate database and makes order records separate and resolute so that an error in one area of the system will not corrupt transaction data.

The service in this architecture plays the role of a coordinator between the user and the inventory. It is based on the inter-service communication through synchronous REST API calls to Product Service to confirm the availability of items and their prices, and confirm an order. This makes the system consistent in data across various service boundaries and loosely coupled.


### Product Service (Rust)


 product-service is a central microservice that maintains the product catalog including storage and retrieval and update of product data like names, description and price. It is coded in Python and the Flask web framework, which was probably selected because Flask is rather lightweight and simple to use when writing RESTful APIs. It is a stack that can be quickly developed, and is highly readable, which makes it ideal in specialized services that specialize in CRUD (Create, Read, Update, Delete) operations on the larger ecosystem.

Architecture and Communication In the microservices architecture, the product-service is a downstream provider of resources. It works autonomously and has its own database (usually an instance of MongoDB as recommended by the laboratory environment) to guarantee loose coupling and data separation. It communicates with other services, i.e. an API Gateway or a frontend service, mainly using synchronous RESTful APIs via HTTP. Upon a request to this service being sent to it or made by one of the users or another service (such as an Order service) to check the availability of items or retrieve some information, this service processes the request and sends the relevant JSON data back.

### Store Front (Vue.js)


Purpose and Technology Stack The store-front is the user interface of the application and it is the one that shows the product catalog and allows the checkout process. It is constructed based on Vue.js, a progressive JavaScript framework due to its reactivity and capability to build a dynamic and one-page experience. This enables real time, speedy front end responding with live updates as the user engages with the store.

Architecture and Communication In the microservices architecture, this service would serve as the client facing layer, which summarizes the information to the end user. It is based on the asynchronous HTTP calls to communicate with the backend. In particular, it retrieves item information in the product-service and transmits transaction information to the order-service to complete purchases, the interface between the user and the application internal logic.

---

