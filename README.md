# PrimeTrade Backend Assignment

## Project Overview
This is the backend for the PrimeTrade Backend Developer Internship Assignment.  
It includes a secure, scalable REST API with JWT authentication, role-based access, and CRUD operations for a secondary entity (Tasks).

---

## Features

- User Registration & Login with hashed passwords
- JWT Authentication for protected routes
- Role-Based Access Control (User/Admin)
- CRUD APIs for Tasks
- API versioning and error handling
- Database: MongoDB with Mongoose
- Postman collection for testing all APIs

---

## Tech Stack

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT for authentication
- Nodemon for development

---

## How to Run Locally

1. Install dependencies:
```
npm install
```

2. Make sure MongoDB is running locally (`mongod`)

3. Create a `.env` file in the project root with the following:
```
PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/primetrade
JWT_SECRET=your_secret
```

4. Start the server:
```
npm run dev
```

5. Test APIs using Postman (see exported collection)

---

## Project Structure

```
primetrade-backend/
 ├── src/
 │   ├── config/       # Database connection
 │   ├── controllers/  # Route logic
 │   ├── middleware/   # Auth, error handling
 │   ├── models/       # Mongoose schemas
 │   ├── routes/       # API endpoints
 │   └── server.js     # Entry point
 ├── .gitignore
 ├── package.json
 ├── package-lock.json
 └── README.md
```

---

## Postman Collection

- All endpoints (Register, Login, Tasks CRUD) are included  
- Use **Bearer Token** for protected routes  

---

## Scalability Notes

- Can be scaled using **microservices architecture**  
- **Redis caching** can be added for performance  
- **Load balancers** can handle high traffic  
- Structured to **easily add new modules**
