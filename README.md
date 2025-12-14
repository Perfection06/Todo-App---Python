# Todo Application – Full Stack Engineer Take-Home Assessment

## 📌 Overview
This is a full-stack Todo application built as part of a take-home assessment.

The application allows users to:
- Create a todo task with title and description
- View the 5 most recent incomplete tasks
- Mark tasks as completed
- Hide completed tasks automatically

---

## 🧱 Tech Stack

### Frontend
- React (Vite)
- TypeScript
- Tailwind CSS
- shadcn/ui

### Backend
- PHP (Apache)
- REST-style API
- JSON communication

### Database
- MySQL

### Containerization
- Docker
- Docker Compose

---

## 🏗️ Architecture

```text
Frontend (React)
    ↓ HTTP (JSON)
Backend (PHP API)
    ↓ SQL
MySQL Database
```

Each layer is independent and communicates via well-defined interfaces.

---

## 📁 Project Structure

```text
todo_app/
├── backend/
│   ├── index.php
│   ├── db.php
│   ├── routes/
│   └── Dockerfile
│
├── frontend/
│   ├── src/
│   ├── Dockerfile
│   └── package.json
│
├── database/
│   └── init.sql
│
├── docker-compose.yml
└── README.md
```

---

## 🚀 Running the Application (Without Docker)

### Backend
- Place the project inside `htdocs`
- Start Apache & MySQL using XAMPP
- Backend API runs at:
```text
http://localhost/todo_app/backend
```

### Frontend
```bash
cd frontend
npm install
npm run dev
```

Open:
```text
http://localhost:5173
```

---

## 🐳 Running the Application (With Docker)

> Docker configuration is provided to ensure reproducibility.
> Due to local Windows environment limitations, Docker was not run locally,
> but the setup is complete and can be executed in any Docker-supported environment.

```bash
docker compose up --build
```

Services:
- Frontend → http://localhost:5173
- Backend → http://localhost:8000
- MySQL → port 3306

---

## 🧪 Testing

### Backend
- Basic PHPUnit tests are provided for API functionality.

### Frontend
- Manual testing performed through UI interactions.

---

## 🔒 Notes

- No authentication was required as per assessment scope.
- Input validation is handled at both frontend and backend levels.

---

