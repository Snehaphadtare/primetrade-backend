# PrimeTrade Backend Developer Internship Assignment

## 📌 Project Overview
This project is a full-stack demonstration built for the **PrimeTrade Backend Developer Internship Assignment**.

It includes a **secure, scalable REST API** with JWT authentication and role-based access, along with a **basic React frontend UI** to demonstrate API usage.

---

## 🚀 Features

### 🔐 Authentication & Authorization
- User Registration & Login
- Password hashing using bcrypt
- JWT-based authentication
- Role-based access control (User / Admin)

### 📦 Task Management (CRUD)
- Create tasks (Authenticated users)
- View tasks
  - Users see only their own tasks
  - Admins can see all tasks
- Update tasks (Owner/Admin only)
- Delete tasks (Owner/Admin only)

### 🛠 Backend Capabilities
- RESTful API design with proper status codes
- API versioning (`/api/v1`)
- Input validation & error handling
- MongoDB database with Mongoose ODM
- Scalable project structure

### 🎨 Frontend (React)
- Register & Login UI
- JWT-protected dashboard
- Create & delete tasks
- Displays real-time API responses
- Clean, minimal UI for demonstration

---

## 🧰 Tech Stack

**Backend**
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- bcrypt
- Nodemon

**Frontend**
- React.js (Single-page demo UI)

---

## 📂 Project Structure

primetrade-backend/
│
├── src/
│ ├── config/
│ │ └── db.js
│ ├── controllers/
│ ├── middlewares/
│ ├── models/
│ ├── routes/
│ ├── app.js
│ └── server.js
│
├── frontend/ (React demo UI)
│
├── .env
├── package.json
├── README.md


---

## ⚙️ Environment Variables

Create a `.env` file in the root directory:

PORT=5000
MONGO_URI=mongodb://127.0.0.1:27017/primetrade
JWT_SECRET=primetrade_secret_key


---

## ▶️ How to Run Locally

### 1️⃣ Clone Repository
```bash
git clone <your-github-repo-url>
cd primetrade-backend
2️⃣ Install Backend Dependencies
npm install
3️⃣ Start Backend Server
npm run dev
Server runs on:

http://localhost:5000
4️⃣ Run Frontend
cd frontend
npm install
npm start
Frontend runs on:

http://localhost:3000
