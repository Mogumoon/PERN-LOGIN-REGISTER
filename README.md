# 🔐 PERN Login & Register Authentication

A full-stack authentication project using **PERN Stack**
(PostgreSQL, Express, React, Node.js) with **JWT Cookie-based Authentication**.

## 🚀 Tech Stack

### Backend
- Node.js
- Express.js
- PostgreSQL
- bcrypt
- jsonwebtoken
- cookie-parser
- dotenv
- cors

### Frontend
- React (Vite)
- React Router
- Axios
- Tailwind CSS

## 📂 Project Structure

```
PERN-LOGIN-REGISTER/
│
├── backend/
│   ├── config/db.js
│   ├── middleware/auth.js
│   ├── routes/auth.js
│   ├── server.js
│   └── package.json
│
├── frontend/
│   ├── src/
│   │   ├── api/axios.js
│   │   ├── components/Navbar.jsx
│   │   ├── pages/Login.jsx
│   │   ├── pages/Register.jsx
│   │   ├── App.jsx
│   │   └── main.jsx
│   └── package.json
│
└── README.md
```

## ⚙️ Backend Setup

### Install
```bash
cd backend
npm install
```

### Environment
```env
PORT=5000
DATABASE_URL=postgresql://username:password@localhost:5432/db_name
JWT_SECRET=your_jwt_secret
CLIENT_URL=http://localhost:5173
```

### Database
```sql
CREATE TABLE users (
  id SERIAL PRIMARY KEY,
  name VARCHAR(100),
  email VARCHAR(255) UNIQUE,
  password TEXT
);
```

### Run Backend
```bash
npm run dev
```

## 💻 Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

## 🔑 Auth Flow
- Register
- Login (JWT stored in HTTP-only cookie)
- Logout (cookie cleared)
- Protected routes using middleware

## 👨‍💻 Author
Mogumoon
