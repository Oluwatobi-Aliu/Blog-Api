Blog Api
The Blog Api is basically a back-end for Simple Blog Web Application. This API consists of Login, Logout and Authentication endpoints in addition to back-end endpoints for Create, Update, View, Delete Posts, Users, Posts and a Category endpoint to organise  and sort blog posts by categories.

Table of Contents
Authors and Contributors
How to deploy the app?
Resources Used
Goals
1. Author
I, Aliu Oluwatobi developed this Application.

2. How to check the app ?
Follow the steps below to check back-end API :

Postman Collection Link : "not yet completed"
URL - "not yet developed" (Only Create User and Login, these two requests don't require authentication, all other requests require authentication.)
Request Routes:

Create User

Type: POST
Endpoint: URL/api/users/register
Request Body: { "username": "Tobi21", "email": "xyz@gmail.com", "password": "xyz" }

User Login

Type: POST
Endpoint: URL/api/users/login
Request Body: { "username": "Tobi21", "password": "xyz" }

New Post Entry

Type: POST
Endpoint: URL/api/posts/
Request Body: { "title": "Web3.0 for techies", "description": "Let's start with why "Web3.0"..., categories: [Technology] }

Fetch All Posts

Type: GET
Endpoint: URL/api/posts/
(Set Request Header)

Fetch Individual Post

Type: GET
Endpoint: URL/api/posts/:id (e.g: id -> 5969902e3989c2063b925d4a)
(Set Request Header)

Fetch All Categories

Type: GET
Endpoint: URL/api/categories

Create a new Category

Type: POST
Endpoint: URL/api/categories/
Request body: { "name": "Technology" }

Update Individual Post

Type: PUT
Endpoint: URL/api/posts/:id (e.g: id -> 5969902e3989c2063b925d4a)

Update Individual User

Type: PUT
Endpoint: URL/api/users/:id (e.g: id -> 5969902e3989c2063b925d4a)

Delete Individual Post

Type: DELETE
Endpoint: URL/api/posts/:id (e.g: id -> 5969902e3989c2063b925d4a)

Delete Individual User

Type: DELETE
Endpoint: URL/api/users/:id (e.g: id -> 5969902e3989c2063b925d4a)

`
3. Tools
Node.js is used as the scripting language for server side programming .
Modules used in the API from npm. These modules are:
express, path, body-parser, JWT, mongoose, bcrypt, multer
Database : MongoDB
4. Goals
 Create a back-end API with Node.js
 Use MongoDB as a No Sql Database
 Write Test using Mocha and Chai
Give a attaractive front-end look with React