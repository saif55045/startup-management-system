# 🏢 Startup Management System

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=black)](https://react.dev/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white)](https://www.mongodb.com/)

A full-stack startup management platform built for the **Zevenz** organization. This system streamlines founder onboarding, attendance tracking, activity logging, team chat, subscription plan management, and account reactivation — all within a modern, responsive dashboard.

---

## ✨ Features

- **👥 Founder Management** — Register, onboard, and manage startup founders with profile customization and image cropping.
- **📅 Attendance Tracking** — Automated daily attendance logging with cron job synchronization and resync capabilities.
- **📋 Activity Logging** — Track and log daily activities per founder for performance reviews.
- **💬 Real-Time Chat** — Socket.IO-powered messaging system for team communication.
- **📊 Dashboard Analytics** — Visual summary of team performance, attendance rates, and activity metrics.
- **💳 Subscription Plans** — Manage billing cycles and plan tiers for startup memberships.
- **🔄 Account Reactivation** — Handle deactivation/reactivation workflows with request approval.
- **🔐 Secure Authentication** — JWT-based login, password reset, rate limiting, input sanitization, and Helmet headers.

---

## 🛠️ Tech Stack

| Layer | Technologies |
|-------|-------------|
| **Frontend** | React 19, Vite, React Router v7, Axios, Socket.IO Client |
| **Backend** | Node.js 18+, Express 5, Mongoose, Socket.IO |
| **Database** | MongoDB |
| **Auth** | JWT, bcrypt.js |
| **Security** | Helmet, CORS, express-rate-limit, express-mongo-sanitize |
| **Scheduling** | node-cron (attendance sync) |
| **Deployment** | Vercel (Frontend) |

---

## 📦 Getting Started

### Prerequisites
- Node.js v18 or higher
- MongoDB Atlas account or local MongoDB instance

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/saif55045/Zevenz_Startup_Management.git
   cd Zevenz_Startup_Management
   ```

2. **Set up the Backend:**
   ```bash
   cd backend
   npm install
   cp .env.example .env
   # Edit .env with your MongoDB URI, JWT secret, etc.
   npm start
   ```

3. **Set up the Frontend:**
   ```bash
   cd frontend
   npm install
   npm run dev
   ```

4. **Seed initial data (optional):**
   ```bash
   cd backend
   npm run seed
   ```

---

## 📐 Project Structure

```
Zevenz_Startup_Management/
├── backend/
│   ├── src/
│   │   ├── controllers/      # Route handlers (auth, chat, attendance, etc.)
│   │   ├── middleware/        # Auth & validation middleware
│   │   ├── models/            # Mongoose schemas (User, Plan, Activity, etc.)
│   │   ├── routes/            # Express route definitions
│   │   └── jobs/              # Cron jobs (attendance sync)
│   ├── server.js              # Express + Socket.IO server entry
│   └── package.json
├── frontend/
│   ├── src/
│   │   ├── components/        # Reusable UI (Sidebar, Topbar, ImageCropper)
│   │   ├── pages/             # Page views (Dashboard, Auth, etc.)
│   │   └── App.jsx            # Root component
│   └── package.json
└── README.md
```

---

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.


## 🖼️ Screenshots

![Screenshot](assets/Screenshot%202026-06-18%20214046.png)

![Screenshot](assets/Screenshot%202026-06-18%20214159.png)

![Screenshot](assets/Screenshot%202026-06-18%20214249.png)

![Screenshot](assets/Screenshot%202026-06-18%20214333.png)

![Screenshot](assets/Screenshot%202026-06-18%20214421.png)

![Screenshot](assets/Screenshot%202026-06-18%20214457.png)


