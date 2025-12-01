# MERN Stack Internship Project: Learning Management System (LMS)

This repository serves as the central hub for the Learning Management System (LMS) project developed during my 16-day in-house MERN Stack Internship. It documents the architecture, setup instructions, core technologies used, and tracks the daily progress and mastery of concepts.

## 1. Project Overview

The goal of this project is to build a fully functional, scalable, and secure Learning Management System (LMS) using the MERN stack, encompassing features for Admin, Instructor, and Student roles.

| Feature | Description |
|--------|-------------|
| Project Type | Full-Stack Web Application |
| Target Audience | Students, Instructors, and Administrators |
| Core Functionality | Course CRUD (Create, Read, Update, Delete), Role-Based Authentication, Secure Deployment |
| Deployment Platform | AWS (EC2, S3, CloudFront) |

## 2. Core Technology Stack

This project is built using the MERN stack, along with industry-standard tools and practices.

| Layer | Technology | Key Concepts Mastered |
|-------|------------|------------------------|
| Database (M) | MongoDB / Mongoose | Schema Design, CRUD Operations, Data Validation, MongoDB Atlas connection |
| Backend (E) | Express.js | RESTful API, Routing, Middleware, CORS, Env Variables |
| Frontend (R) | React.js | Components, Hooks, Router v6, Context API, Form Validation |
| Runtime (N) | Node.js | Server Setup, Async Programming, NPM, PM2 |
| Styling | Tailwind CSS | Utility-First CSS, Responsive Design, Dark Mode |
| Security | JWT, bcrypt | Authentication, Hashing, Authorization |
| DevOps | AWS (EC2, S3, CloudFront), GitHub Actions | Deployment, CI/CD |

## 3. Installation & Local Setup

### Prerequisites
- Node.js (v18+)
- MongoDB (local or Atlas)
- Git & GitHub

### Steps

#### Clone the Repository
```bash
git clone [YOUR_REPOSITORY_URL]
cd MERN-Internship-LMS
```

#### Backend Setup
```bash
cd backend/
npm install
```

Create `.env`:
```
PORT=5000
MONGO_URI="YOUR_MONGO_URI"
JWT_SECRET="YOUR_SECRET_KEY"
```

Start server:
```bash
npm start
```

#### Frontend Setup
```bash
cd ../frontend/
npm install
```

Create `.env`:
```
VITE_REACT_APP_API_URL="http://localhost:5000/api"
```

Start client:
```bash
npm run dev
```

## 4. RESTful API Endpoints Documentation

| Resource | Method | Endpoint | Description | Status |
|----------|--------|----------|-------------|--------|
| Authentication | POST | /api/auth/register | Registers new user | COMPLETED |
| Authentication | POST | /api/auth/login | Returns JWT token | COMPLETED |
| Courses | GET | /api/courses | Fetch all courses | IN PROGRESS |
| Courses | POST | /api/courses | Create new course | TODO |
| Users | GET | /api/users/profile | Get user details | TODO |

## 5. 16-Day Internship Mastery Log

### Phase 1: Frontend (Days 1–8)

| Day | Topic | Status |
|-----|--------|---------|
| 1 | MERN Overview | ✅ Completed |
| 2 | HTML5 | ⬜ To Do |
| 3 | CSS3 + Tailwind | ⬜ To Do |
| 4 | JavaScript Fundamentals | ⬜ To Do |
| 5 | Modern JS (ES6+) | ⬜ To Do |
| 6 | React Components | ⬜ To Do |
| 7 | Hooks & State Mgmt | ⬜ To Do |
| 8 | Routing & Forms | ⬜ To Do |

### Phase 2: Backend (Days 9–11)

| Day | Topic | Status |
|-----|--------|---------|
| 9 | Node.js & Express | ⬜ To Do |
| 10 | MongoDB & Mongoose | ⬜ To Do |
| 11 | Authentication & Security | ⬜ To Do |

### Phase 3: Deployment (Days 12–16)

| Day | Topic | Status |
|-----|--------|---------|
| 12 | Cloud Concepts | ⬜ To Do |
| 13 | AWS EC2 Deployment | ⬜ To Do |
| 14 | AWS S3 & CloudFront | ⬜ To Do |
| 15 | CI/CD | ⬜ To Do |
| 16 | Monitoring & Optimization | ⬜ To Do |

## 6. Project Architecture Overview

- **Frontend:** React + Tailwind, communicates via REST API  
- **Backend:** Node.js, Express.js  
- **Database:** MongoDB with Mongoose  
- **Deployment:**  
  - Backend → AWS EC2  
  - Frontend → AWS S3 + CloudFront  

## 7. How to Contribute

1. Create feature branch:
```bash
git checkout -b feat/new-feature
```

2. Commit:
```bash
git commit -m "feat: add new dashboard component"
```

3. Push:
```bash
git push origin feat/new-feature
```

4. Create Pull Request.
