# 📝 Notes API

A RESTful backend API for managing users and notes with authentication, authorization, file uploads, and email functionality.

Built with **Node.js**, **Express**, and **MongoDB** following a modular MVC architecture.

---

## 🚀 Features

### Authentication & Users

- User registration and login
- JWT authentication
- Session management
- Password reset via email
- Protected routes
- User profile management

### Notes Management

- Create notes
- Update notes
- Delete notes
- Get all user notes
- Search and filter notes
- Note validation

### Additional Features

- File upload with Multer
- Cloudinary image storage
- Email notifications
- Request logging
- Centralized error handling
- Input validation

---

## 🛠 Tech Stack

### Backend

<p align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/express/express-original.svg" width="45"/>
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/mongodb/mongodb-original.svg" width="45"/>
</p>

- Node.js
- Express.js
- MongoDB
- Mongoose

### Libraries & Services

- JWT
- bcrypt
- Joi
- Multer
- Cloudinary
- Nodemailer
- Morgan
- dotenv

---

## 🏗 Architecture

The project follows an MVC-based architecture:

```
src/
│
├── controllers/
│   ├── authController.js
│   ├── notesController.js
│   └── userController.js
│
├── models/
│   ├── user.js
│   ├── note.js
│   └── session.js
│
├── routes/
│   ├── authRoutes.js
│   ├── notesRoutes.js
│   └── userRoutes.js
│
├── middleware/
│   ├── authenticate.js
│   ├── multer.js
│   ├── logger.js
│   └── errorHandler.js
│
├── services/
│
├── utils/
│
└── server.js
```

---

## 🔐 Authentication Flow

- User registration
- Password hashing
- JWT token generation
- Session storage
- Protected API endpoints
- Password reset through email

---

## 📚 API Endpoints

### Authentication

| Method | Endpoint | Description |
|---|---|---|
| POST | `/auth/register` | Create user account |
| POST | `/auth/login` | User login |
| POST | `/auth/logout` | User logout |
| POST | `/auth/reset-password` | Reset password |

---

### Notes

| Method | Endpoint | Description |
|---|---|---|
| GET | `/notes` | Get user notes |
| POST | `/notes` | Create note |
| PATCH | `/notes/:id` | Update note |
| DELETE | `/notes/:id` | Delete note |

---

## ⚙️ Installation

Clone repository:

```bash
git clone https://github.com/Vl-as/nodejs-hw.git
```

Install dependencies:

```bash
npm install
```

Create `.env` file:

```env
PORT=
MONGODB_URI=
JWT_SECRET=

CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

SMTP_HOST=
SMTP_PORT=
SMTP_USER=
SMTP_PASSWORD=
```

Start development server:

```bash
npm run dev
```

---

## 🎯 What I Learned

During this project I improved my backend development skills:

- Building REST APIs with Express.js
- Designing scalable project architecture
- Working with MongoDB and Mongoose
- Implementing authentication and authorization
- Creating custom middleware
- Handling file uploads
- Sending emails from backend
- Writing validation and error handling logic

---

## 🔮 Future Improvements

- Add automated tests
- Add Swagger API documentation
- Add Docker support
- Improve API documentation
- Deploy backend service

---

## 👨‍💻 Author

**Vl-as**

🐙 GitHub: https://github.com/Vl-as
💼 LinkedIn: [Volodymyr Asieiev](https://www.linkedin.com/in/volodymyr-asieiev/)
💬 Telegram: [@vasvv](https://t.me/vasvv)
