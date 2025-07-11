# RESTful Task Manager API

A backend API built using **Node.js** and **Express** that supports **user authentication** and **task management (CRUD operations)**. The API uses **JWT** for secure authentication and **MongoDB** for data persistence.

---

## 🔧 Features

- ✅ User registration & login (JWT-based authentication)
- ✅ Create, read, update, and delete (CRUD) tasks
- ✅ Secure routes with middleware
- ✅ Password hashing using bcrypt
- ✅ MongoDB with Mongoose for schema modeling
- ✅ Organized route structure and controllers

---

## 🛠 Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB (via Mongoose)
- **Authentication:** JWT (JSON Web Tokens)
- **Password Security:** bcrypt
- **Environment Config:** dotenv

---

## 📁 Project Structure


├── config
│ └── db.js
├── controllers
│ ├── authController.js
│ └── taskController.js
├── middleware
│ └── authMiddleware.js
├── models
│ ├── User.js
│ └── Task.js
├── routes
│ ├── authRoutes.js
│ └── taskRoutes.js
├── .env
├── .gitignore
├── app.js
├── package.json
├── package-lock.json
└── README.md


---

## 🚀 Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/your-username/RESTful-Task-Manager-API.git
cd RESTful-Task-Manager-API
```

Install Dependencies:
```
npm install
```

Create a .env file in the root folder and add:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

Run the Server:
```
npm run dev
```


📬 API Endpoints:
🔐 Auth Routes
```
POST /api/auth/register – Register a new user

POST /api/auth/login – Log in a user and receive a JWT token
```

📋 Task Routes (protected)
Requires Authorization: Bearer <token> in headers

```
GET /api/tasks – Get all tasks for the user

POST /api/tasks – Create a new task

PUT /api/tasks/:id – Update a task

DELETE /api/tasks/:id – Delete a task
```

Example Request:
```
POST /api/auth/register
Content-Type: application/json

{
  "username": "manoj",
  "email": "manoj@example.com",
  "password": "yourpassword"
}
```

📂 GitHub
🔗 https://github.com/manojnath18/RESTful-Task-Manager-API

🙋‍♂️ Author
Manoj Nath
🔗 http://www.linkedin.com/in/manoj-nath-sm29



