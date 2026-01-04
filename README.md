# ✅ Smart ToDo API 

**A robust RESTful backend system built for secure and efficient task management.**

---

## 📖 Overview
The **Smart ToDo API** provides a secure foundation for managing daily tasks. It features a scalable NoSQL architecture and industry-standard JWT authentication to ensure user data remains private and organized. Developed as part of the **Intern Technical Assessment: Engineering & Data**.

## 🚀 Key Features
* **User Authentication:** Secure registration and login using **JSON Web Tokens (JWT)**.
* **Database Integration:** Seamless connection with **MongoDB** (NoSQL) for high-performance data storage.
* **Full CRUD Functionality:** Dedicated endpoints to Create, Read, Update, and Delete tasks.
* **Middleware Protection:** Private routes that require a valid authentication token.

## 🛠️ Technology Stack
* **Runtime:** Node.js
* **Framework:** Express.js
* **Database:** MongoDB (NoSQL)
* **Security:** JWT (JSON Web Tokens) & Bcrypt (Password Hashing)

## 🔌 API Endpoints Reference

### Authentication
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/auth/signup` | Register a new user account |
| `POST` | `/api/auth/login` | Authenticate and receive a JWT token |

### Task Management (Requires Token)
| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/api/tasks` | Create a new task |
| `GET` | `/api/tasks` | Retrieve all tasks for the authenticated user |
| `PUT` | `/api/tasks/:id` | Update a specific task's details or status |
| `DELETE` | `/api/tasks/:id` | Permanently remove a task |

## ⚙️ Installation & Execution

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/theshovan/smart-todo-api.git]
    cd smart-todo-api
    ```

2.  **Install Dependencies:**
    ```bash
    npm install
    ```

3.  **Environment Setup:**
    Create a `.env` file in the root and add:
    ```env
    PORT=5000
    MONGO_URI=your_mongodb_connection_string
    JWT_SECRET=your_super_secret_key
    ```

4.  **Run the Server:**
    ```bash
    npm start
    ```
    *The server will be running at `http://localhost:5000`.*

## 📄 Submission Materials
* **Postman Collection:** A JSON file for testing all endpoints is located in the `/docs` folder.
* **Source Code:** Fully organized modular structure following industry best practices.

---
**Developed by:** [Shovan Bera](https://github.com/theshovan)
