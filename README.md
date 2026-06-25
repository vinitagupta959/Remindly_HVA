# 🧠 Remindly – AI-Powered Spaced Repetition Learning Platform

> **A Full-Stack MERN application built during the HyperVerge Academy (HVA) Hackathon to improve long-term learning through Spaced Repetition, AI-powered evaluations, adaptive quizzes, and gamification.**

---

## 📌 About the Project

Remindly is a smart learning platform designed to help users remember concepts more effectively using the **Spaced Repetition** learning technique. Instead of simply storing notes, the platform schedules revisions at scientifically proven intervals, evaluates users' understanding using AI, and reinforces learning through adaptive quizzes.

This project was developed during the **HyperVerge Academy (HVA) Hackathon** as a team project. I primarily contributed as a **Backend Developer**, where I designed and developed REST APIs, implemented authentication, integrated MongoDB, built the spaced repetition algorithm, and integrated Google Gemini AI for intelligent learning features.

---

# ✨ Features

## 🔐 Authentication

* User Registration & Login
* JWT-based Authentication
* Secure Password Hashing using bcrypt
* Protected Routes

## 📚 Topic Management

* Create learning topics
* Edit and delete topics
* View revision history
* Track learning progress

## 🧠 Spaced Repetition

* Automatic revision scheduling
* Day 1 Revision
* Day 7 Revision
* Day 30 Revision
* Memory strength updates after every revision

## 🤖 AI Features

* AI-generated quizzes using Google Gemini
* AI evaluation of user explanations
* Adaptive quiz difficulty
* Instant AI feedback

## 📝 Quiz System

* Multiple Choice Questions
* Adaptive Difficulty Levels
* Instant Score Calculation
* Quiz Result History

## 🏆 Gamification

* Points System
* Learning Streaks
* Global Leaderboard
* Performance Rankings

## 📊 Dashboard

* Today's Revisions
* Overdue Topics
* Upcoming Revisions
* Progress Summary

## 📱 Responsive Design

* Desktop
* Tablet
* Mobile Friendly

---

# 👩‍💻 My Contribution

### Backend Development

* Designed RESTful APIs using Express.js
* Implemented JWT Authentication & Authorization
* Integrated MongoDB using Mongoose
* Created Topic, User and QuizResult Models
* Built CRUD operations for Topics
* Developed Spaced Repetition Scheduling Logic
* Implemented Quiz Result APIs
* Built Leaderboard APIs
* Integrated Google Gemini API
* Added Secure Password Hashing using bcrypt
* Implemented User-wise Data Isolation
* Configured Environment Variables and CORS

### Frontend Integration

* Connected Backend APIs with React
* Implemented Authentication Flow
* Integrated Dashboard
* Connected Topic Management Pages
* Integrated Quiz APIs
* Fixed API Integration Issues

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
* JWT
* bcrypt
* Google Gemini API

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
│   └── package.json
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
    └── package.json
```

---

# ⚙️ Installation

## Clone Repository

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

Create a `.env` file:

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/remindly
JWT_SECRET=your-secret-key
GEMINI_API_KEY=your-gemini-api-key
CORS_ORIGIN=http://localhost:5173
NODE_ENV=development
```

Run Backend

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

# 🔄 Application Flow

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
 AI Evaluation (Gemini)
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

| Stage           | Day    |
| --------------- | ------ |
| Topic Created   | Day 0  |
| First Revision  | Day 1  |
| Second Revision | Day 7  |
| Third Revision  | Day 30 |

The revision schedule automatically adapts based on quiz performance and user progress.

---

# 🏆 Points System

```
Base Points = 10

Easy Difficulty   = ×1
Medium Difficulty = ×1.5
Hard Difficulty   = ×2

Final Score =
Base Points × (Quiz Score / Total Questions) × Difficulty Multiplier
```

---

# 🔒 Security

* JWT Authentication
* Password Hashing using bcrypt
* Protected API Routes
* Environment Variables
* User-wise Data Isolation
* Secure CORS Configuration

---

# 🚀 Future Improvements

* Dark Mode
* Study Groups
* Topic Categories & Tags
* Email Reminder System
* Push Notifications
* Analytics Dashboard
* Topic Import & Export
* Mobile App (React Native)

---

# 📄 License

This project is licensed under the **MIT License**.

---

# 👩‍💻 Author

**Vinita Gupta**

**Backend Developer | MERN Stack Developer**

GitHub: https://github.com/vinitagupta959

---

⭐ If you found this project helpful, don't forget to give it a **Star**.
