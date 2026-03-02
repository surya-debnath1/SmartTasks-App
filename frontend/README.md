# SmartTasks – Mobile Application (Frontend)

This folder contains the React Native (Expo) mobile application for SmartTasks.

The app communicates with the backend REST API for authentication and task operations.

---

## 📱 Features

- User Registration
- User Login (JWT Authentication)
- Create Task
- View Tasks
- Update Task Status
- Delete Task
- Search Tasks
- Filter by Status
- Logout
- Secure token storage using AsyncStorage

---

## 🛠 Tech Stack

- React Native
- Expo
- Expo Router
- TypeScript
- Axios
- AsyncStorage

---

## 🚀 Running the App

Navigate to frontend folder:

```
cd frontend
```

Install dependencies:

```
npm install
```

Start the app:

```
npx expo start
```

Use:
- Expo Go (Android/iOS)
- Android Emulator
- iOS Simulator

---

## 🔗 Backend Configuration

Ensure the API base URL inside:

```
src/config/api.ts
```

points to:

```
https://smart-task-manager-backend-gfx6.onrender.com/api
```

---

## 🎯 Implementation Highlights

- Context API for authentication state management
- File-based routing using Expo Router
- Axios interceptor for automatic token injection
- Modular component structure