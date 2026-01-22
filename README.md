# PrimeTrade Backend Project

## Overview
This project is a backend-focused implementation with a simple frontend UI built to demonstrate secure API design, authentication, and CRUD functionality. The application follows REST principles and is structured to support scalability and future expansion.

---

## Features

### Authentication & Authorization
- User registration and login
- Password hashing using bcrypt
- JWT-based authentication
- Role-based access control (user and admin)

### Task Management
- Create tasks (authenticated users)
- View tasks
  - Users can access only their own tasks
  - Admin users can access all tasks
- Update tasks (owner or admin)
- Delete tasks (owner or admin)

### Backend Architecture
- RESTful APIs with proper HTTP status codes
- API versioning using `/api/v1`
- Centralized error handling
- MongoDB database with Mongoose
- Modular and scalable folder structure

### Frontend
- Basic React UI for API interaction
- User registration and login
- JWT-protected dashboard
- Create and delete tasks
- Displays API responses clearly

---

## Tech Stack

**Backend**
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Token (JWT)
- bcrypt
- Nodemon

**Frontend**
- React.js

---

## Project Structure

primetrade-backend/
├── src/
│ ├── config/
│ ├── controllers/
│ ├── middlewares/
│ ├── models/
│ ├── routes/
│ ├── app.js
│ └── server.js
│
├── frontend/
├── package.json
├── README.md


---

## Environment Setup

Create a `.env` file in the root directory:

PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/primetrade
JWT_SECRET=primetrade_secret_key


---

## Running the Project

### Backend
```bash
npm install
npm run dev
The backend server runs on:

http://localhost:5000
Frontend
cd frontend
npm install
npm start
The frontend runs on:

http://localhost:3000
API Endpoints
Authentication
POST /api/v1/auth/register

POST /api/v1/auth/login

Tasks (Protected)
GET /api/v1/tasks

POST /api/v1/tasks

PUT /api/v1/tasks/:id

DELETE /api/v1/tasks/:id

Scalability Considerations
Stateless authentication using JWT

Modular architecture for easy feature expansion

Can be extended with caching, load balancing, or containerization
