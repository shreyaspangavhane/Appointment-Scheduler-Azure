# 🗓️ Appointment Scheduling Web App

A full-stack web application for booking and managing appointments — perfect for doctors, salons, clinics, and service businesses. Built with **React**, **Node.js**, and **MySQL**, this app features secure authentication, calendar integration, CRUD operations, and email reminders.

---


## ⚙️ Features

- ✅ Secure Signup/Login with JWT
- 🗓️ Book, View, Reschedule, or Cancel Appointments
- 🔔 Email Notifications for Confirmations and Reminders
- 📅 Calendar UI for Date Selection
- 🧑‍💼 Separate Dashboards for Users and Admins *(Optional)*

---

## 🧰 Tech Stack

### Frontend:
- React.js
- React Router
- Axios
- Tailwind CSS or Custom CSS

### Backend:
- Node.js
- Express.js
- MySQL (via mysql2)
- JWT Authentication
- NodeMailer for Emails

---

## 📁 Folder Structure

```
appointment-app/
├── backend/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── config/
│   ├── utils/
│   ├── server.js
│   └── .env
│
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── components/
│   │   ├── services/
│   │   ├── App.jsx
│   │   └── index.js
│   └── public/
│
├── README.md
└── .gitignore
```

---

## 🚀 Local Setup Instructions

### 🔧 Prerequisites

- Node.js (v18+)
- MySQL Server
- Git

---

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/appointment-app.git
cd appointment-app
```

---

### 2. Setup MySQL Database

1. Login to MySQL:
```bash
mysql -u root -p
```

2. Create a database:
```sql
CREATE DATABASE appointment_db;
```

3. (Optional) Import schema if provided.

---

### 3. Backend Setup

```bash
cd backend
npm install
```

> Create a `.env` file inside the `backend/` folder:

```env
PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_mysql_password
DB_NAME=appointment_db
JWT_SECRET=your_jwt_secret
EMAIL_USER=your_email@example.com
EMAIL_PASS=your_email_app_password
```

Start the backend:
```bash
npm start
```

---

### 4. Frontend Setup

```bash
cd ../frontend
npm install
npm start
```

The frontend will run on [http://localhost:3000](http://localhost:3000)

---

## 📡 API Overview

| Method | Route | Function |
|--------|-------|----------|
| POST | `/api/auth/signup` | Register a user |
| POST | `/api/auth/login` | Login user |
| GET | `/api/appointments` | Get user appointments |
| POST | `/api/appointments/book` | Book an appointment |
| PUT | `/api/appointments/:id` | Reschedule |
| DELETE | `/api/appointments/:id` | Cancel |

---

## 🛡️ Security

- Passwords are hashed using bcrypt.
- JWT used for session management.
- Protected routes using middleware.
- Basic input validation on both frontend and backend.

---

## 🧑‍💻 Author

**Shreyas Sanjay Pangavhane**  
📧 Email: shreyaspangavhane2022@gmail.com  
🎓 4rd Year Computer Engineering Student  
📍 SCOE, Kopargaon

---



## 📜 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.
