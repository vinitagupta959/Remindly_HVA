# 🧠 Remindly – AI-Powered Spaced Repetition Learning Platform

> **A Full-Stack MERN application built during the HyperVerge Academy (HVA) Hackathon to improve long-term learning through Spaced Repetition, AI-powered evaluations, adaptive quizzes, and gamification.**

🌐 **Live Demo:** https://hva-remindly-1.onrender.com

> Create a new account using the **Sign Up** page to explore all features.

---

# 📌 About the Project

Remindly is an AI-powered learning platform that helps users retain knowledge through the **Spaced Repetition** technique. Instead of simply storing notes, the application schedules revisions at scientifically proven intervals, evaluates users' understanding using AI, and reinforces learning with adaptive quizzes.

This project was developed during the **HyperVerge Academy (HVA) Hackathon** as a collaborative team project. I primarily contributed as a **Backend Developer**, where I designed and implemented REST APIs, JWT authentication, MongoDB integration, the spaced repetition algorithm, quiz management, leaderboard functionality, and Google Gemini AI integration.

---

# ✨ Features

### 🔐 Authentication

* User Registration & Login
* JWT Authentication
* Secure Password Hashing with bcrypt
* Protected Routes

### 📚 Topic Management

* Create, Update and Delete Topics
* View Topic Details
* Revision History
* Track Learning Progress

### 🧠 Spaced Repetition

* Automatic Revision Scheduling
* Day 1 Revision
* Day 7 Revision
* Day 30 Revision
* Memory Strength Tracking

### 🤖 AI Features

* AI-generated Quizzes
* AI-based Explanation Evaluation
* Adaptive Quiz Difficulty
* Instant Feedback using Google Gemini

### 📝 Quiz System

* Multiple Choice Questions
* Difficulty Levels (Easy, Medium, Hard)
* Quiz History
* Performance Tracking

### 🏆 Gamification

* Points System
* Learning Streaks
* Global Leaderboard
* Rank Tracking

### 📊 Dashboard

* Today's Revisions
* Overdue Topics
* Upcoming Topics
* Learning Summary

### 📱 Responsive UI

* Desktop
* Tablet
* Mobile Friendly

---

# 🛠 Tech Stack

## Frontend

* React 18
* React Router DOM
* Vite
* Context API
* Fetch API
* CSS

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication
* bcrypt
* Google Gemini API
  ---

# 👩‍💻 My Contribution

As a **Backend Developer** in the HVA Hackathon team, I worked on the core backend architecture and API development.

### Backend Development

* Designed RESTful APIs using Express.js
* Implemented JWT Authentication & Authorization
* Integrated MongoDB using Mongoose ODM
* Created User, Topic and QuizResult Models
* Developed CRUD APIs for Topic Management
* Built the Spaced Repetition Scheduling Logic
* Implemented Quiz Result APIs
* Developed Leaderboard APIs
* Integrated Google Gemini API
* Configured Environment Variables
* Added Secure Password Hashing using bcrypt
* Implemented User-specific Data Isolation
* Configured CORS

### Frontend Integration

* Connected React with Backend APIs
* Implemented Authentication Flow
* Integrated Dashboard APIs
* Connected Topic Management
* Integrated Quiz APIs
* Fixed API Integration Issues

---

# 📁 Project Structure

```text
remindly-app/
│
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── utils/
│   ├── server.js
│   ├── package.json
│   └── .env.example
│
└── frontend/
    ├── src/
    │   ├── components/
    │   ├── context/
    │   ├── pages/
    │   ├── services/
    │   ├── styles/
    │   ├── App.jsx
    │   └── main.jsx
    ├── package.json
    └── .env.example
```

---

# ⚙️ Installation

## Clone the Repository

```bash
git clone https://github.com/vinitagupta959/HVA_Remindly.git
cd HVA_Remindly
```

---

## Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file.

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/remindly
JWT_SECRET=your-secret-key
GEMINI_API_KEY=your-gemini-api-key
CORS_ORIGIN=http://localhost:5173
NODE_ENV=development
```

Start Backend

```bash
npm run dev
```

---

## Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

Frontend

```text
http://localhost:5173
```

Backend

```text
http://localhost:5000
```

---

# 🔗 API Endpoints

## Authentication

| Method | Endpoint         |
| ------ | ---------------- |
| POST   | /api/auth/signup |
| POST   | /api/auth/signin |
| GET    | /api/auth/me     |

## Topics

| Method | Endpoint                     |
| ------ | ---------------------------- |
| GET    | /api/topics                  |
| POST   | /api/topics                  |
| GET    | /api/topics/:id              |
| PUT    | /api/topics/:id              |
| DELETE | /api/topics/:id              |
| POST   | /api/topics/:id/mark-revised |

## AI

| Method | Endpoint                       |
| ------ | ------------------------------ |
| POST   | /api/ai/generate-quiz          |
| POST   | /api/ai/evaluate-explanation   |
| POST   | /api/ai/generate-adaptive-quiz |

## Quiz Results

| Method | Endpoint                   |
| ------ | -------------------------- |
| POST   | /api/quiz-results          |
| GET    | /api/quiz-results/:topicId |

## Leaderboard

| Method | Endpoint         |
| ------ | ---------------- |
| GET    | /api/leaderboard |

---

# 🔄 Application Workflow

```text
User Registration/Login
          │
          ▼
     Dashboard
          │
          ▼
     Create Topic
          │
          ▼
 Write Explanation
          │
          ▼
 AI Evaluation
          │
          ▼
 Adaptive Quiz
          │
          ▼
 Earn Points
          │
          ▼
 Leaderboard
          │
          ▼
 Scheduled Revision
```

---

# 🧠 Spaced Repetition Schedule

| Stage           | Schedule |
| --------------- | -------- |
| Topic Creation  | Day 0    |
| First Revision  | Day 1    |
| Second Revision | Day 7    |
| Third Revision  | Day 30   |

The revision schedule automatically adapts based on quiz performance and user progress.

---

# 🏆 Points System

```text
Base Points = 10

Easy Difficulty   = ×1
Medium Difficulty = ×1.5
Hard Difficulty   = ×2

Final Points =
Base Points × (Score / Total Questions) × Difficulty Multiplier
```

---

# 🔒 Security

* JWT Authentication
* Password Hashing using bcrypt
* Protected Routes
* Secure Environment Variables
* User-specific Data Isolation
* CORS Protection

---

# 🚀 Deployment

| Service  | Platform      |
| -------- | ------------- |
| Frontend | Render        |
| Backend  | Render        |
| Database | MongoDB Atlas |

---

# 🔮 Future Improvements

* Dark Mode
* Study Groups
* Topic Tags & Categories
* Email Reminders
* Push Notifications
* Advanced Analytics Dashboard
* Topic Export & Import
* Mobile Application (React Native)

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👩‍💻 Author

**Vinita Gupta**

Backend Developer | MERN Stack Developer

**GitHub:** https://github.com/vinitagupta959

---

⭐ **If you like this project, don't forget to give it a Star!**
