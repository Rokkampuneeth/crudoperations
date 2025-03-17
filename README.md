Introduction
A RESTful API allows seamless communication between clients and servers using HTTP methods. Node.js and Express provide a lightweight and efficient framework to build scalable APIs. This guide covers setting up a basic CRUD API to perform Create, Read, Update, and Delete operations.

 Project Overview
The project is designed to demonstrate RESTful API principles using Node.js and Express. The API supports:

POST: Create a new resource.
GET: Retrieve all or specific resources.
PUT: Update an existing resource.
DELETE: Remove a resource.


Prerequisites
Before starting, ensure you have the following installed:
Node.js: Required to run JavaScript server-side.
Postman or cURL: To test API endpoints.
A code editor


Installation & Setup
1️ .Clone the repository: git clone <repo_url> and navigate to the project folder.
2️ .Install dependencies: Run npm install to install Express.
3️. Start the server: Run npm start to launch the API on http://localhost:5000/.


Method	    Endpoint	            Description
POST:	  /api/resource	        Create a new resource
GET:      /api/resource	        Retrieve all resources
GET:	  /api/resource/:id	    Retrieve a specific resource
PUT:      /api/resource/:id	    Update a resource
DELETE:   /api/resource/:id	     Delete a resource

API Implementation
Setting up Express Server: Initialize Express and configure middleware.
Defining Routes: Use the express.Router() module to define RESTful endpoints.
Implementing Controller Logic: Store data temporarily and handle CRUD operations.
Connecting Routes: Mount routes to the main application using app.use('/api', apiRoutes)

Testing the API
Use Postman  to send HTTP requests.
Example: To create a resource, send a POST request with JSON data.
Retrieve data with a GET request to /api/resource.
Update or delete resources using PUT and DELETE requests.
