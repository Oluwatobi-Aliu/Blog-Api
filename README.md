# Blog Api
The Blog Api is a back-end api for Simple Blog Web Application. This API consists of Login and Authentication endpoints in addition to back-end endpoints for Create, Update, View, Delete Posts, Users, Posts and a Category endpoint to organise  and sort blog posts by categories.

# Table of Contents
1. [Author](#1-author)
2. [Check the API](#2-check-the-api)
3. [Run the API](#3-run-the-api)
4. [Resources Used](#4-resources-used)
5. [Goals](#5-goals)

## 1. Author
   I, Aliu Oluwatobi developed this Application.

## 2. Check the API
   Follow the steps below to check back-end API :

   + Postman Collection Link : "not yet completed"
   + URL - "not yet developed" (Only Create User and Login, these two requests don't require authentication, all other requests require authentication.)
### Request Routes:

**Create User**

+ Type: POST
+ Endpoint: URL/api/users/register
+ Request Body: { "username": "Tobi21", "email": "xyz@gmail.com", "password": "xyz" }

**User Login**

+ Type: POST
+ Endpoint: URL/api/users/login
+ Request Body: { "username": "Tobi21", "password": "xyz" }

**New Post Entry**

+ Type: POST
+ Endpoint: URL/api/posts/
+ Request Body: { "title": "Web3.0 for techies", "description": "Let's start with why "Web3.0...", categories: [Technology] }

**Fetch All Posts**

+ Type: GET
+ Endpoint: URL/api/posts/

**Fetch Individual**

+ Type: GET
+ Endpoint: URL/api/posts/:id (e.g: id -> 5969902e3989c2063b925d4a)

**Fetch All Categories**

* Type: GET
* Endpoint: URL/api/categories

**Create a new Category****

+ Type: POST
+ Endpoint: URL/api/categories/
+ Request body: { "name": "Technology" }

**Update Individual Post**

+ Type: PUT
+ Endpoint: URL/api/posts/:id (e.g: id -> 5969902e3989c2063b925d4a)

**Update Individual User**

+ Type: PUT
+ Endpoint: URL/api/users/:id (e.g: id -> 5969902e3989c2063b925d4a)

**Delete Individual Post**

+ Type: DELETE
+ Endpoint: URL/api/posts/:id (e.g: id -> 5969902e3989c2063b925d4a)

**Delete Individual User**

+ Type: DELETE
+ Endpoint: URL/api/users/:id (e.g: id -> 5969902e3989c2063b925d4a)

## 3. Run the API
1. Download the source code and navigate to the project's folder
2. Enter the project's folder using your preferred IDE or terminal
3. Run the following commands
   ``` 
   $ npm install
   $ npm start
   ```
## 4. Resources Used

Node.js is used as the scripting language for server side programming .

Modules used in the API from npm. 

These modules are:
express, path, body-parser, JWT, mongoose, bcrypt, multer

Database : MongoDB

## 5. Goals
+ [x] Create a back-end API with Node.js
+ [x] Use MongoDB as a No Sql Database
+ Write Test using Mocha and Chai
+ Give a attaractive front-end look with React
