# 🌊 TaskFlow - Team Task Manager

![MERN Stack](https://img.shields.io/badge/MERN-Stack-blue?style=for-the-badge&logo=mongodb)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Node.js](https://img.shields.io/badge/Node.js-Backend-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-Backend-000000?style=for-the-badge&logo=express&logoColor=white)

TaskFlow is a premium full-stack team task management application built with the **MERN** stack (MongoDB, Express.js, React, Node.js). It empowers teams to create projects, assign tasks, and track progress seamlessly using a visual Kanban board, all wrapped in a stunning modern UI.

🚀 **Live Demo:** [View TaskFlow on Railway](https://team-task-manager-production-2131.up.railway.app)

---

## ✨ Premium UI: macOS Glassmorphism
The application features a highly refined **macOS Glass** design aesthetic:
- **Vibrant Backgrounds:** A dynamic gradient mesh wallpaper serves as the foundation.
- **Advanced Translucency:** Components utilize deep backdrop blurs (`blur(24px) saturate(180%)`) to create realistic frosted glass effects.
- **Precision Glass Edges:** Crisp 1px highlight borders simulate light refracting off physical glass panels.
- **Fluid Micro-Animations:** Soft hover states and dynamic drop shadows make the UI feel alive and responsive.

## 🛠️ Key Features

* **Authentication & Security:** Secure signup/login using JWT (JSON Web Tokens) and bcryptjs password hashing.
* **Role-Based Access Control (RBAC):**
  * **Admin:** Full privileges to create/delete projects, assign tasks, and manage team members.
  * **Member:** Access to view assigned projects and update task statuses.
* **Project Management:** Create active projects, assign due dates, and invite members via email.
* **Kanban & List Views:** Visualize workflows with dynamic Kanban columns (To Do, In Progress, Completed) or view a structured tabular list.
* **Live Dashboard:** Get a bird's-eye view of your team's performance with real-time statistics on active, completed, and overdue tasks.

---

## 💻 Tech Stack

**Frontend:**
- React 18 & React Router v6
- Axios (API Client)
- Custom CSS (Glassmorphism UI System)

**Backend:**
- Node.js & Express.js
- MongoDB & Mongoose (ODM)
- JSON Web Tokens (JWT) for secure state persistence

---

## 🚀 Local Setup Instructions

### Prerequisites
- Node.js (v18+)
- MongoDB (Local instance or MongoDB Atlas cluster)

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/team-task-manager.git
cd team-task-manager
```

### 2. Backend Setup
```bash
cd backend
npm install
```
Create a `.env` file in the `backend` directory:
```env
PORT=5001
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_super_secret_jwt_key
FRONTEND_URL=http://localhost:3000
```
Start the backend server:
```bash
npm run dev
```

### 3. Frontend Setup
Open a new terminal window:
```bash
cd frontend
npm install
```
Start the React development server:
```bash
npm start
```
The app will open automatically at `http://localhost:3000`.

---

## ☁️ Deployment

This project is configured for seamless deployment on **Railway.app**.
1. **Database:** Create a MongoDB service on Railway (or use Atlas).
2. **Backend:** Deploy the `/backend` directory and provide the `MONGO_URI` and `JWT_SECRET` environment variables.
3. **Frontend:** Deploy the `/frontend` directory. Ensure `src/utils/api.js` points to your live backend URL. Railway will automatically detect React and build the static assets.

---

*Designed and developed as a complete MERN stack solution.*
