📇 Contact Manager API

Secure RESTful API built with Node.js, Express, and MongoDB (Mongoose) to manage user contacts. It supports user authentication, CRUD operations, and protected routes using JWT tokens.

🚀 Features

✅ Express server and project setup

✅ Express Router and custom middleware

✅ MongoDB database integration with Mongoose

✅ Error handling with express-async-handler

✅ CRUD operations for contacts (Create, Read, Update, Delete)

✅ User authentication (Register & Login)

✅ Password hashing and comparison using bcrypt

✅ JWT token signing and verification

✅ Protected routes and user authorization

✅ Relationship handling (User → Contacts)

✅ API testing using Thunder Client

🛠️ Tech Stack

Backend: Node.js, Express.js

Database: MongoDB (Mongoose ODM)

Authentication: JSON Web Tokens (JWT), bcrypt

Testing: Thunder Client / Postman

📁 Project Setup

Clone the repository:

git clone https://github.com/ireneiroha/Contact_Manager_api.git
cd contact-manager-api


Install dependencies:

npm install


Create an .env file:

PORT=5000
MONGO_URI=your_mongodb_connection_string
ACCESS_TOKEN_SECRET=your_jwt_secret


Run the server:

npm run dev

📚 Folder Structure
project-root/
│
├── controllers/
│   ├── contactController.js
│   └── userController.js
│
├── middleware/
│   ├── validateTokenHandler.js
│   └── errorHandler.js
│
├── models/
│   ├── contactModel.js
│   └── userModel.js
│
├── routes/
│   ├── contactRoutes.js
│   └── userRoutes.js
│
├── config/
│   └── dbConnection.js
│
├── server.js
└── .env

🔐 Authentication Flow

User Registration (/api/users/register)

Hash password using bcrypt

Save user to MongoDB

User Login (/api/users/login)

Compare entered password with hashed password

Generate JWT token using jsonwebtoken

Protected Routes

Use custom middleware (validateTokenHandler.js)

🧰 Commands
Command	Description
npm run dev	Run server with Nodemon
npm start	Run server normally
npm install	Install dependencies

Verify JWT to access private resources
