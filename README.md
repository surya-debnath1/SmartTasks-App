# 📱 SmartTasks App – Full Stack Task Management System

SmartTasks is a full-stack mobile task management application developed using React Native (Expo) for the frontend and Node.js with MongoDB for the backend.

The project demonstrates secure authentication, RESTful API integration, user-specific data isolation, and Android APK deployment as part of a Software Engineering academic submission.

---

## 📌 Project Description

SmartTasks allows registered users to manage their personal tasks securely.

Each user can:

- Create tasks
- Update task status
- Delete tasks
- Search tasks by title
- Filter tasks by status
- Access only their own task data
- Log in and log out securely

All task operations are protected using JWT authentication.

---

## 🏗 Application Architecture

```
Mobile App (React Native + Expo)
           ↓
REST API (Node.js + Express)
           ↓
MongoDB Database
```

- The mobile application communicates with the backend using HTTP requests.
- JWT is used for stateless authentication.
- MongoDB stores users and tasks.
- Backend routes are protected using middleware.
- Task ownership validation ensures security.

---

## 🛠 Technology Stack

### Frontend (Mobile Application)
- React Native
- Expo
- Expo Router
- TypeScript
- Axios
- AsyncStorage

### Backend (API Server)
- Node.js
- Express.js
- MongoDB
- Mongoose
- JSON Web Token (JWT)
- bcryptjs
- CORS

---

## 📂 Repository Structure

```
SmartTasks_App/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   ├── app.js
│   └── server.js
│
├── frontend/
│   ├── app/
│   ├── src/
│   ├── assets/
│   └── app.json
│
└── README.md
```

---

## 🌐 Backend Deployment

The backend API is deployed on Render.

Production API Base URL:

https://smart-task-manager-backend-gfx6.onrender.com/api

The mobile application connects directly to this deployed API.

---

## 📥 Android APK Download

Download the latest Android build below:

👉 [Download SmartTasks APK](https://github.com/surya-debnath1/SmartTasks-App/releases/download/v1.0.0/SmartTasks.apk)

After downloading:

1. Enable installation from unknown sources (if required).
2. Install the APK on your Android device.
3. Open the application and test all features.

---

## 🚀 Running Locally

### Backend Setup

```
cd backend
npm install
npm run dev
```

Create a `.env` file inside backend:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
```

---

### Frontend Setup

```
cd frontend
npm install
npx expo start
```

Use Expo Go to test on a physical device.

---

## 📦 Building Android APK

The APK is generated using Expo Application Services (EAS):

```
eas build -p android --profile preview
```

After build completion:
- Download the `.apk`
- Upload to GitHub Releases
- Update the APK link above

---

## 🔐 Security Implementation

- Password hashing using bcrypt
- JWT-based authentication
- Protected API routes
- Ownership validation for tasks
- Environment variables for sensitive credentials
- MongoDB schema validation

---

## 🎓 Academic Objective

This project was developed to demonstrate:

- REST API design
- Secure authentication implementation
- MVC backend architecture
- Database modeling
- State management in React Native
- Mobile UI development
- Deployment process

---

## 👨‍💻 Author

Surya Debnath