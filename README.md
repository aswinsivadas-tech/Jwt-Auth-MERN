# Jwt-Auth-MERN

A robust, production-ready Authentication System built with the MERN stack (MongoDB, Express, React, Node.js). This project implements secure stateless authentication using JSON Web Tokens (JWT) and HttpOnly cookies, along with Redux Toolkit for state management.

## 🚀 Features

- **Full MERN Stack**: React (with Vite) frontend, Node/Express backend, and MongoDB database.
- **Secure Authentication**: JWT-based stateless authentication.
- **State Management**: Redux Toolkit integrated on the frontend.
- **Modern Styling**: Styled beautifully with Tailwind CSS v4.
- **API Ready**: Pre-configured RESTful API routes for Registration, Login, User Profile, and Logout.
- **Developer Friendly**: Uses `concurrently` to run both client and server from a single command.

## 💻 Tech Stack

- **Frontend**: React 19, Vite, Tailwind CSS v4, React Router, Redux Toolkit, Axios, Lucide React (Icons).
- **Backend**: Node.js, Express.js, MongoDB (Mongoose), JWT (jsonwebtoken), bcryptjs, cookie-parser.

## 🛠️ Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- MongoDB account/cluster or local MongoDB server

### Installation

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone <https://github.com/aswinsivadas-tech/Jwt-Auth-MERN>
   cd Jwt-Auth-MERN
   ```

2. **Install all dependencies** (Frontend, Backend, and Root):
   ```bash
   npm run install-all
   ```

3. **Configure Environment Variables**:
   Navigate to the `server` directory and ensure your `.env` file is set up correctly:
   ```env
   PORT=5000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   JWT_EXPIRE=15m
   JWT_REFRESH_SECRET=your_refresh_secret
   JWT_REFRESH_EXPIRE=7d
   NODE_ENV=development
   ```

### Running the Application

You can start both the frontend and backend servers simultaneously from the root directory using a single command:

```bash
npm run dev
```

- **Frontend**: `http://localhost:5173`
- **Backend**: `http://localhost:5000`

## 📡 API Endpoints

The following authentication routes are available at `http://localhost:5000/api/auth`:

| Method | Endpoint    | Description                     | Access   |
| :----- | :---------- | :------------------------------ | :------- |
| POST   | `/register` | Register a new user             | Public   |
| POST   | `/login`    | Authenticate user & get token   | Public   |
| GET    | `/me`       | Get current user profile data   | Private  |
| GET    | `/logout`   | Logout and clear cookies        | Public   |

## 📄 License

This project is licensed under the ISC License.
