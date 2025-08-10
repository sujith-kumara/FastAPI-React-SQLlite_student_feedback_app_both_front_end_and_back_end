# 🎓 Student Feedback Manager

![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-0.95+-teal.svg)
![React](https://img.shields.io/badge/React-18-blue.svg)
![SQLite](https://img.shields.io/badge/SQLite-3-lightgrey.svg)
![Docker](https://img.shields.io/badge/Docker-ready-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)

A full-stack app where **students** can submit course feedback and **teachers** can view it.  
Built with **FastAPI** (backend) + **React** (frontend), with **free-tier hosting** on Render/Vercel.  

---

## 🚀 Live Demo

- **Backend (FastAPI + SQLite)** → [Live API](https://fastapi-react-sqllite-student-feedback.onrender.com)  
- **Frontend (React)** → [Live App](https://fastapi-react-frontend.vercel.app/)

---

## 📜 Problem Statement

> Create a simple feedback management app:
> - Students can submit feedback for a course.
> - Teachers can view all submitted feedback.

---

## ✨ Features

### Backend (FastAPI)
- Store feedback (**name, email, feedback text**)
- Retrieve all feedback entries
- Uses SQLite 
- Dockerised for easy deployment

### Frontend (React)
- Form for submitting feedback
- Table/List view to display feedback
- Responsive and minimal UI

---

## 🏗️ Tech Stack

- **Backend:** FastAPI, SQLite, Uvicorn
- **Frontend:** React, Axios
- **Deployment:** Render / Railway (backend), Vercel / Netlify (frontend)
- **Docker:** Containerized backend

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/sujith-kumara/FastAPI-React-SQLlite_student_feedback_app_both_front_end_and_back_end.git
cd FastAPI-React-SQLlite_student_feedback_app_both_front_end_and_back_end


## 2️⃣ Backend Setup (FastAPI)

### Local Setup
```bash
cd backend
python -m venv venv
source venv/bin/activate   # Windows → venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload


Backend will run at → http://127.0.0.1:8000


### Docker Setup
'''bash
cd backend
docker build -t feedback-backend .
docker run -p 8000:8000 feedback-backend

### Frontend Setup (React)
'''bash
cd frontend
npm install
npm start
Frontend will run at → http://localhost:3000


📦 API Endpoints
Method	Endpoint	Description
POST	/feedback	Submit feedback
GET	/feedback	Retrieve all entries

FastAPI-React-SQLlite_student_feedback_app_both_front_end_and_back_end/
│
├── backend/           # FastAPI backend
│   ├── main.py
│   ├── requirements.txt
│   └── Dockerfile
│
├── frontend/          # React frontend
│   ├── src/
│   ├── package.json
│   └── public/
│
└── README.md

