<div align="center">
  <h1>🌊 TaskFlow</h1>
  <p><strong>A Premium, Enterprise-Grade Team Task Management Platform</strong></p>

  <br />
  <a href="https://team-task-manager-production-2131.up.railway.app">
    <img src="https://img.shields.io/badge/🚀_CLICK_HERE_TO_VIEW_LIVE_APP-6366f1?style=for-the-badge&logo=railway&logoColor=white" alt="Live Demo" />
  </a>
  <br /><br />

  <p>
    <img src="https://img.shields.io/badge/MERN-Stack-blue?style=flat-square&logo=mongodb" alt="MERN Stack" />
    <img src="https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React" />
    <img src="https://img.shields.io/badge/Node.js-Backend-339933?style=flat-square&logo=nodedotjs&logoColor=white" alt="Node.js" />
    <img src="https://img.shields.io/badge/Express.js-REST_API-000000?style=flat-square&logo=express&logoColor=white" alt="Express" />
    <img src="https://img.shields.io/badge/JWT-Authentication-black?style=flat-square&logo=jsonwebtokens" alt="JWT" />
  </p>
</div>

---

## 🎯 Overview

**TaskFlow** is a full-stack, responsive team collaboration tool designed to streamline project workflows. Built from the ground up using the **MERN** stack, it demonstrates the ability to architect complex state management on the frontend while securely managing relational data models in a NoSQL database on the backend.

> 💡 **For Recruiters:** This project was built to showcase clean architecture, secure RESTful API design, complex state management in React, and a meticulous eye for premium UI/UX.

---

## 🏗️ Technical Architecture & Highlights

### 1. Robust Authentication & RBAC (Role-Based Access Control)
- **JWT Implementation:** Secure, stateless authentication flow using JSON Web Tokens.
- **Password Security:** Salted and hashed passwords utilizing `bcryptjs` before persisting to MongoDB.
- **Admin vs. Member Tiers:** Full role-based authorization middleware protecting API routes. Only Admins can execute destructive actions or modify user permissions.

### 2. State-of-the-Art UI/UX Engineering
- **macOS Glassmorphism System:** Engineered a custom, lightweight CSS design system relying heavily on advanced `backdrop-filter: blur(24px) saturate(180%)` CSS properties over a dynamic, responsive gradient mesh.
- **Custom Components:** No bulky UI libraries (like Bootstrap or Material UI) were used. Every component (Kanban boards, Modals, Cards) was built from scratch to demonstrate deep CSS architecture skills.
- **Smooth Micro-Interactions:** Utilized highly optimized CSS transitions for hover states, ensuring 60fps performance without JavaScript overhead.

### 3. Backend & Database Design
- **Relational Data in NoSQL:** Implemented advanced Mongoose `.populate()` queries to efficiently fetch referenced data across `Users`, `Projects`, and `Tasks` collections.
- **RESTful Principles:** The Express backend strictly adheres to REST principles, ensuring predictable, standard HTTP verb usage (GET, POST, PUT, DELETE) and standard HTTP status code responses.
- **Centralized Error Handling:** Axios interceptors on the frontend catch unauthorized (`401`) errors and seamlessly redirect unauthenticated users without breaking the UI flow.

---

## 🚀 Live Demonstration

> ### 🌐 [Click Here to Access the Live Application](https://team-task-manager-production-2131.up.railway.app)
> *The application is deployed as a high-performance microservice architecture on Railway.*
> 
> **💡 Testing Tip:** *To fully explore the platform, create two separate accounts (or use two different browsers) to test the real-time project invitations and Role-Based Access controls!*

---

## 💻 Tech Stack Deep Dive

| Layer | Technologies Used | Purpose |
| :--- | :--- | :--- |
| **Frontend** | React 18, React Router v6, Axios | Component-based UI, Client-side routing, Promise-based HTTP client. |
| **Backend** | Node.js, Express.js | Event-driven backend server, REST API routing. |
| **Database** | MongoDB, Mongoose | Schema-based document storage, Data validation. |
| **Security** | JWT, bcryptjs, CORS | Session management, Cryptography, Cross-Origin Resource Sharing. |
| **Deployment**| Railway | CI/CD, Containerized Cloud Deployment. |

---

## ⚙️ Running Locally

### Prerequisites
- Node.js (v18+)
- MongoDB Atlas URI or Local MongoDB instance

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/team-task-manager.git
   cd team-task-manager
   ```

2. **Initialize the Backend**
   ```bash
   cd backend
   npm install
   ```
   Create a `.env` file in the `backend` directory:
   ```env
   PORT=5001
   MONGO_URI=mongodb+srv://<your_cluster_uri>
   JWT_SECRET=your_super_secret_jwt_key
   FRONTEND_URL=http://localhost:3000
   ```
   Start the Express server: `npm run dev`

3. **Initialize the Frontend**
   ```bash
   cd ../frontend
   npm install
   npm start
   ```

---

<div align="center">
  <p><i>Crafted with passion for clean code and beautiful design.</i></p>
</div>
