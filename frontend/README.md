 📚 E-Learning Platform

A full-stack e-learning platform where students can register, enroll in courses, watch video modules, take quizzes, and earn certificates.

This project is structured into a **backend (Node.js/Express + MongoDB)** and a **frontend (React)**, ensuring scalability, maintainability, and a clear separation of concerns.

---

## 🚀 Features

### 🔐 Authentication & Authorization

* User registration & login with JWT.
* Role-based access (e.g., student, admin).
* Protected routes (frontend & backend).

### 🎓 Courses & Modules

* Browse and enroll in courses.
* Stream video modules with progress tracking.
* Course details with modular content.

### 📝 Quizzes

* Take quizzes for modules/courses.
* Track quiz scores & attempt history.
* Show quiz results with feedback.

### 📜 Certificates

* Auto-generate certificates after course completion.
* Download certificates in PDF format.

### 📊 Dashboard

* Student dashboard with progress charts.
* Visual progress tracking for courses & quizzes.

---

## 📂 Project Structure

```
elearning-platform/
├── backend/        # Node.js + Express API
├── frontend/       # React client
└── README.md       # Project documentation
```

---

### 🔧 Backend (`backend/`)

* **config/** → Database & JWT configuration
* **controllers/** → Logic for authentication, courses, modules, quizzes, certificates
* **middleware/** → Authentication & validation middlewares
* **models/** → Mongoose models (`User`, `Course`, `Module`, `Quiz`, `Certificate`)
* **routes/** → API routes for different features
* **utils/** → Helper functions & PDF generator
* **seeders/** → Database seed script
* **uploads/** → Storage for videos & certificates
* **app.js / server.js** → Express server setup

➡️ Runs on **Node.js + Express + MongoDB**

---

### 🎨 Frontend (`frontend/`)

* **public/** → Entry HTML file
* **src/** → Main React codebase

  * **components/** → Reusable UI components, organized by feature (auth, courses, modules, quizzes, dashboard, certificates, common)
  * **context/** → React context for authentication state
  * **services/** → API service wrappers for backend communication
  * **utils/** → Utility functions/constants
  * **App.jsx / index.js** → Main React app entry

➡️ Built with **React + Context API + Axios**

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository

```bash
git clone https://github.com/Abdurehman-Kero/E-learning-platform.git
cd elearning-platform
```

### 2️⃣ Backend Setup

```bash
cd backend
npm install
```

* Create a `.env` file in `backend/` with:

  ```env
  PORT=5000
  MONGO_URI=your_mongodb_uri
  JWT_SECRET=your_secret_key
  ```

* Run the server:

  ```bash
  npm start
  ```

### 3️⃣ Frontend Setup

```bash
cd frontend
npm install
npm start
```

* The frontend will run on [http://localhost:3000](http://localhost:3000).
* Backend runs on [http://localhost:5000](http://localhost:5000).

---

## 🛠️ Tech Stack

* **Frontend:** React, Context API, Axios, Chart.js
* **Backend:** Node.js, Express, MongoDB, Mongoose, JWT, Multer
* **Other:** PDFKit (certificate generation), bcrypt (password hashing)

---
