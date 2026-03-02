# 📱 SmartTasks – Full Stack Task Management Application

SmartTasks is a full-stack mobile task management system built using React Native (Expo) for the frontend and Node.js with MongoDB for the backend.

This project demonstrates secure authentication, RESTful API development, protected routes, user-level data isolation, and Android APK deployment as part of a Software Engineering academic submission.

---

## 📌 Overview

SmartTasks enables users to:

- Register and log in securely using JWT authentication
- Create, update, and delete personal tasks
- Filter tasks by status (Pending, In Progress, Completed)
- Search tasks by title
- Access only their own task data
- Log out securely

All API endpoints are protected and validated on the backend.

---

## 🏗 System Architecture

```
Mobile App (React Native + Expo)
           ↓
REST API (Node.js + Express)
           ↓
MongoDB Database
```

- The frontend communicates with the backend using REST APIs.
- JWT ensures stateless authentication.
- MongoDB stores user and task data.
- Ownership validation prevents unauthorized access.

---

## 🛠 Technology Stack

### Frontend
- React Native
- Expo
- Expo Router
- TypeScript
- Axios
- AsyncStorage

### Backend
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
├── backend/        → REST API (Node.js + Express)
├── frontend/       → Mobile Application (Expo)
└── README.md       → Project Overview
```

---

## 🌐 Backend Deployment

The backend API is deployed on Render.

Production Base URL:

https://smart-task-manager-backend-gfx6.onrender.com/api

---

## 📥 Android APK Download

Download the latest Android build below:

👉 [Download SmartTasks APK](https://github.com/surya-debnath1/SmartTasks-App/releases/download/v1.0.0/SmartTasks.apk)

---

## 🚀 Running Locally

### Backend

```
cd backend
npm install
npm run dev
```

Create a `.env` file inside `backend/`:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
PORT=5000
```

---

### Frontend

```
cd frontend
npm install
npx expo start
```

Scan QR code using Expo Go.

---

## 📦 APK Build Command

```
eas build -p android --profile preview
```

After build:
- Download APK
- Upload to GitHub Releases
- Update link above

---

## 🔐 Security Highlights

- Password hashing with bcrypt
- JWT-based authentication
- Protected API routes
- Ownership validation for tasks
- Environment variable configuration

---

## 🎓 Academic Context

Developed as part of a Software Engineering academic assessment to demonstrate:

- REST API design
- Secure authentication flow
- MVC backend structure
- Database schema modeling
- Mobile UI implementation
- Deployment process

---

## 👨‍💻 Author

Surya Debnath