# SmartTasks – Backend API

This folder contains the REST API server for the SmartTasks application.

The backend is responsible for authentication, task management, and secure database operations.

---

## 🛠 Tech Stack

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- bcryptjs
- CORS

---

## 🚀 Installation

Navigate to the backend folder:

```
cd backend
```

Install dependencies:

```
npm install
```

Create a `.env` file:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
```

Start the server:

```
npm run dev
```

Server runs at:

```
http://localhost:5000
```

---

## 🔐 API Endpoints

### Authentication

- POST `/api/users/register`
- POST `/api/users/login`
- GET `/api/users/profile` (Protected)

### Tasks

- POST `/api/tasks` (Protected)
- GET `/api/tasks` (Protected)
- PUT `/api/tasks/:id` (Protected)
- DELETE `/api/tasks/:id` (Protected)

Supports:

- Filtering: `/api/tasks?status=Completed`
- Search: `/api/tasks?search=keyword`

---

## 🔒 Security Features

- Password hashing using bcrypt
- JWT-based route protection
- Ownership validation for task updates/deletes
- Schema validation using Mongoose