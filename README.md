#  Student Grievance Management System (MERN Stack)

##  Project Overview

This is a **web-based Student Grievance Management System** built using the **MERN Stack (MongoDB, Express, React, Node.js)**.
The system allows students to register, log in, and manage their grievances efficiently.

---

##  Features

### 🔐 Authentication

* User Registration
* User Login (JWT आधारित authentication)
* Secure password hashing using bcrypt

###  Grievance Management

* Submit grievance
* View all grievances
* Search grievances by title
* Update grievance
* Delete grievance

###  Security

* Protected routes using JWT
* Only logged-in users can access dashboard
* Error handling (invalid login, duplicate email, unauthorized access)

---

##  Tech Stack

### Frontend:

* React.js
* Axios
* React Router DOM

### Backend:

* Node.js
* Express.js

### Database:

* MongoDB (Mongoose)

---

##  Project Structure

```
grievance-system/
│
├── backend/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── server.js
│   └── .env
│
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   ├── App.js
│   │   └── index.js
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 1️ Clone Repository

```
git clone <your-repo-link>
cd grievance-system
```

---

### 2️⃣ Backend Setup

```
cd backend
npm install
```

Create `.env` file:

```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=secretkey
PORT=5000
```

Run backend:

```
node server.js
```

---

### 3️⃣ Frontend Setup

```
cd frontend
npm install
npm install axios react-router-dom
npm start
```

---

## 🔗 API Endpoints

### Auth APIs

* POST `/api/register`
* POST `/api/login`

### Grievance APIs

* POST `/api/grievances`
* GET `/api/grievances`
* GET `/api/grievances/:id`
* PUT `/api/grievances/:id`
* DELETE `/api/grievances/:id`
* GET `/api/grievances/search?title=xyz`

---

## 🧪 Testing

Use Postman to test APIs:

* Register a user
* Login and get token
* Use token in headers:

```
Authorization: <token>
```

---

## ☁️ Deployment

### Backend:

* Deploy on Render

### Frontend:

* Deploy on Netlify / Render

---

## 📸 Screenshots

(Add screenshots here for better presentation)

---

## 🎯 Conclusion

This project provides a simple and efficient way for students to raise and track grievances.
It ensures transparency, security, and ease of use using modern web technologies.

---

##  Author

**Ashutosh Shukla**
B.Tech CSE (AI & ML)

---

## Notes

* Make sure MongoDB is connected
* Backend should run before frontend
* Token is required for protected routes
