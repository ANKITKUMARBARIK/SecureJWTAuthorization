
# 🔐 SecureJWTAuthorization

A secure and professional authentication and authorization system using **JWT (JSON Web Tokens)**. This system ensures that both **authentication** and **role-based authorization** are effectively implemented. Built with **Node.js** and **Express**, it handles **protected routes** using JWT tokens passed in the **Authorization Bearer header** and restricts access based on user roles.

---

## 📦 Features

- 🧾 User Signup & Login
- 🔐 JWT Token-based Authentication
- 🛡️ Role-Based Authorization (`ADMIN`, `USER`)
- 📩 Token sent via `Authorization: Bearer <token>` header
- 🔒 Protected Routes using Middleware
- ❌ Logout by removing token on client side
- 💻 Clean and modular folder structure

---

## 📁 Project Structure

```
SecureJWTAuthorization/
│
├── controllers/       # Logic for handling requests
├── middleware/        # Authentication and authorization middleware
├── routes/            # API route handlers
├── utils/             # Helper functions
├── .env               # Environment variables
├── server.js          # Application entry point
└── package.json       # Project metadata and dependencies
```

---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/ANKITKUMARBARIK/SecureJWTAuthorization.git
cd SecureJWTAuthorization
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Setup Environment Variables

Create a `.env` file in the root directory:

```
PORT=8000
JWT_SECRET=your_jwt_secret
```

### 4. Start the Server
```bash
npm start
```

---

## 🔐 How It Works

- On login, the server returns a JWT token.
- The client stores the token (e.g., in `localStorage`).
- For protected routes, the client sends the token in the `Authorization` header:
  ```
  Authorization: Bearer <token>
  ```
- Middleware verifies the token and checks for appropriate user roles before granting access.

---

## 🛠️ Tech Stack

- **Node.js**
- **Express.js**
- **jsonwebtoken**
- **dotenv**

---

## 📄 License

This project is licensed under the [GNU License](LICENSE).

---

## 🧑‍💻 Author

Made with ❤️ by [Ankit Kumar Barik](https://github.com/ANKITKUMARBARIK)
