# User Mangaement Backend System.
# Requirements

  Node Js, MangoDB 
  API Documentation-Swagger.
  

                      Curd operations using nodejs and expressjs  and mongodb database


# Folder Structure:
- node_modules/         // Installed dependencies
- models/               // User model definition
- config.js             // Configuration file (e.g., MongoDB URI, JWT secret)
- app.js                // Main application file
- package.json          // Project dependencies and scripts

# Dependencies:
•	express: Web framework for Node.js
•	bcrypt: Library for hashing passwords
•	jsonwebtoken: Library for generating and verifying JWT tokens
•	moment: Library for handling dates and times
•	mongoose: MongoDB object modeling tool
•	body-parser: Middleware for parsing request bodies
•	swagger-jsdoc: Library for generating Swagger documentation
•	swagger-ui-express: Middleware for serving Swagger UI

# Commands to Run the Application:
 Install dependencies:
 
 --npm install –force
 
 Start the application:
 
 --npm start

# Explanation:
# 1.	Setup and Configuration:
•	Required dependencies are imported.
•	MongoDB is connected using the provided URI from the config.js file.
•	JWT secret key is defined.
# 2.	JWT Token Verification Middleware:
•	verifyToken middleware is defined to check the validity of JWT tokens provided in the request headers.
# 3.	Swagger Documentation:
•	Swagger options are defined, including API information, server URL, and component schemas (such as the User schema).
•	Swagger specification is generated using swaggerJsdoc.
•	Swagger UI is served using swaggerUi middleware.
# 4.	API Routes:
•	GET /: Endpoint to check if the server is running.
•	POST /register: Endpoint to register a new user.
•	POST /login: Endpoint to login a user and generate a JWT token.
•	GET /users: Endpoint to retrieve all users (protected by JWT token).
•	GET /getUser/:id: Endpoint to retrieve a user by ID (protected by JWT token).
•	PUT /updateUser/:id: Endpoint to update a user by ID (protected by JWT token).
•	DELETE /deleteUser/:id: Endpoint to delete a user by ID (protected by JWT token).
# 5.	Swagger Documentation for Endpoints:
•	Each endpoint is documented using Swagger annotations, including summaries, descriptions, request/response schemas, and security requirements.
# 6.	Running the Application:
•	The application listens on port 5000 by default.
•	Swagger documentation is accessible at /api-docs endpoint.
# Summary:
Your application is a RESTful API server with user registration, login, CRUD operations on user data, and JWT token authentication. Swagger documentation is provided for each endpoint to facilitate API exploration and testing.


Certainly! CRUD operations refer to Create, Read, Update, and Delete operations, which are fundamental functions for interacting with data in any application. In the context of your Node.js and Express.js application, these operations are typically used to manage user data stored in a MongoDB database. Below is a summary explanation of each CRUD operation:
# 1.	Create (POST /register):
•	The Create operation is used to add new data to the database.
•	In your application, the /register endpoint handles the creation of new user accounts.
•	When a client sends a POST request to this endpoint with user information (email, password, username, phone number, address), the server creates a new user document in the database after validating the input data.
# 2.	Read (GET /users and GET /getUser/:id):
•	The Read operation is used to retrieve existing data from the database.
•	In your application, there are two endpoints for reading user data:
•	/users: Retrieves a list of all users from the database. This endpoint is typically used to display a list of users.
•	/getUser/:id: Retrieves a specific user by their ID from the database. This endpoint is used to fetch detailed information about a particular user.
# 3.	Update (PUT /updateUser/:id):
•	The Update operation is used to modify existing data in the database.
•	In your application, the /updateUser/:id endpoint handles the update of user information.
•	When a client sends a PUT request to this endpoint with the ID of the user to be updated and the updated user data (e.g., username, phone number, address), the server retrieves the user from the database, updates the specified fields, and saves the changes.
# 4.	Delete (DELETE /deleteUser/:id):
•	The Delete operation is used to remove data from the database.
•	In your application, the /deleteUser/:id endpoint handles the deletion of user accounts.
•	When a client sends a DELETE request to this endpoint with the ID of the user to be deleted, the server locates the user in the database, removes the user document, and returns a success message.


Overall, these CRUD operations provide the basic functionality required to manage user data in your Node.js and Express.js application. They allow clients to create, retrieve, update, and delete user records, facilitating efficient data management and interaction with the application.


![WhatsApp Image 2024-04-09 at 23 58 01_d6b76857](https://github.com/Vidya1026/curd/assets/146586310/50df0a5f-51f2-4ea7-a72c-313b5bef3af3)


# New User Registration.

![WhatsApp Image 2024-04-09 at 23 36 54_14530af4](https://github.com/Vidya1026/curd/assets/146586310/6ced118c-c55a-468b-b9b6-a26266869051)

# Existing User Registration.

![WhatsApp Image 2024-04-10 at 00 03 19_03215f61](https://github.com/Vidya1026/curd/assets/146586310/594c0bff-8aca-4241-af17-38f46c20faa8)

# User Login

![WhatsApp Image 2024-04-10 at 00 03 19_cdf9fa35](https://github.com/Vidya1026/curd/assets/146586310/d69f22b7-00a5-4e13-a61a-75747b307972)

![WhatsApp Image 2024-04-10 at 00 03 20_a500fee8](https://github.com/Vidya1026/curd/assets/146586310/058aa605-fd09-40b6-8f12-ca0635bd397c)

# Mongo DB Connection.

![WhatsApp Image 2024-04-10 at 00 03 18_26a24f81](https://github.com/Vidya1026/curd/assets/146586310/36cbcb9f-024e-4ab5-bb12-456a568f9e6d)

![WhatsApp Image 2024-04-10 at 00 03 20_3a06e9cb](https://github.com/Vidya1026/curd/assets/146586310/9ed86b94-239a-4c9e-95e7-477363f9a9af)

![WhatsApp Image 2024-04-10 at 00 41 25_ab927e38](https://github.com/Vidya1026/curd/assets/146586310/0e7b5835-f4bf-4bcb-9b9d-77ba70864ec6)


