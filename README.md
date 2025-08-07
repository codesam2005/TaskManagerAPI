# 📝 Task Manager API

A RESTful Task Manager API built using **Node.js**, **Express**, and **MongoDB (Mongoose)**. This project supports full CRUD operations and includes proper error handling middleware and modular file structure.

---

## 🚀 Features

- ✅ Create a task
- 📄 Read (get all tasks / get a specific task)
- ✏️ Update a task
- ❌ Delete a task
- ⚠️ Proper 404 & custom error handling
- 📦 Environment variable support (`dotenv`)
- 📁 Modular folder structure for scalability

---

## 🔧 Tech Stack

- **Backend:** Node.js, Express.js
- **Database:** MongoDB, Mongoose
- **Middleware:** Custom error handling, async wrapper
- **Dev Tools:** Nodemon, dotenv

---

## 📂 Folder Structure

```
task-manager-api-express-mongoose/
│
├── controllers/
│   └── tasks.js             # Controller logic for tasks
│
├── db/
│   └── connect.js           # MongoDB connection setup
│
├── errors/
│   └── custom-error.js      # Custom error class + factory
│
├── middleware/
│   ├── async.js             # Async wrapper for clean try/catch
│   ├── error-handler.js     # Centralized error handler
│   └── not-found.js         # 404 Not Found middleware
│
├── models/
│   └── Task.js              # Mongoose schema for Task
│
├── public/
│   └── index.html           # Static HTML page (optional)
│
├── routes/
│   └── tasks.js             # Task routes
│
├── .env                     # Environment variables
├── .gitignore
├── app.js                   # Entry point
├── package.json
└── README.md
```

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/codesam2005/TaskManagerAPI.git
cd task-manager-api-express-mongoose
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Setup Environment Variables

Create a `.env` file in the root directory:

```env
PORT=5000
MONGO_URI=mongodb://localhost:27017/taskManagerDB
```

### 4. Start the Server

```bash
npm run dev
```

> Server will run at `http://localhost:5000`

---

## 🛠️ API Endpoints

Base URL: `/api/v1/tasks`

| Method | Route            | Description            |
|--------|------------------|------------------------|
| GET    | `/`              | Get all tasks          |
| POST   | `/`              | Create a new task      |
| GET    | `/:id`           | Get a specific task    |
| PATCH  | `/:id`           | Update a task          |
| DELETE | `/:id`           | Delete a task          |

---

## 📬 Sample Request Body

```json
{
  "name": "Learn Mongoose",
  "completed": true
}
```

---

## 🧪 Testing

You can use **Postman**, **Insomnia**, or **cURL** to test the API.

---

## 📜 License

MIT License. Feel free to use and modify.

---

## 👨‍💻 Author

Built by [Samraj K](https://github.com/codesam2005)
