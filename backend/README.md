# Smart Task Manager - Backend

## Tech Stack

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- bcryptjs

---

## Features

- User Registration
- User Login with JWT Authentication
- Protected Routes
- Task CRUD (Create, Read, Update, Delete)
- Task Filtering by Status
- Task Search by Title
- Ownership Authorization
- Clean MVC Structure

---

## Project Structure

```
src/
├── controllers/
├── routes/
├── models/
├── middleware/
├── config/
└── app.js
```

---

## Installation

1. Clone the repository
2. Navigate to backend folder
3. Install dependencies:

```
npm install
```

4. Create a `.env` file in the root directory:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
```

5. Start the server:

```
npm run dev
```

Server runs at:

```
http://localhost:5000
```

---

## API Endpoints

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
- Search: `/api/tasks?search=backend`

---

## Security

- Password hashing using bcrypt
- JWT-based authentication
- Route protection middleware
- Ownership validation for task updates/deletes