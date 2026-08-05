# 💬 Chat App

![Deployed on Render](https://img.shields.io/badge/Deployed%20on-Render-46E3B7?style=for-the-badge&logo=render&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?style=for-the-badge&logo=node.js&logoColor=white)
![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Socket.io](https://img.shields.io/badge/Socket.IO-Real--Time-010101?style=for-the-badge&logo=socket.io&logoColor=white)

A full-stack **real-time chat application** built with the MERN stack and Socket.IO. Users can sign up, log in, update their profile, and exchange messages with other users in real time.

🔗 **Live Demo**: [https://chat-app-1-vj2h.onrender.com](https://chat-app-1-vj2h.onrender.com)

---

## ✨ Features

- 🔐 **JWT Authentication** — Secure signup, login & logout with HTTP-only cookies
- 💬 **Real-Time Messaging** — Instant messaging powered by Socket.IO
- 🟢 **Online User Indicator** — See who's currently online
- 🖼️ **Profile Picture Upload** — Upload and update avatars via Cloudinary
- 🌗 **32 Themes** — Switch between multiple DaisyUI themes
- 📱 **Fully Responsive** — Works on all screen sizes

---

## 🛠️ Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| React 18 | UI Framework |
| Vite | Build Tool |
| Zustand | State Management |
| TailwindCSS + DaisyUI | Styling & Themes |
| Socket.IO Client | Real-Time Communication |
| Axios | HTTP Requests |
| React Router DOM | Client-Side Routing |

### Backend
| Technology | Purpose |
|---|---|
| Node.js + Express | REST API Server |
| MongoDB + Mongoose | Database |
| Socket.IO | WebSocket Server |
| JWT | Authentication |
| bcryptjs | Password Hashing |
| Cloudinary | Image Storage |
| Cookie-Parser | Cookie Handling |

---

## 📁 Project Structure

```
chat-app/
├── backend/
│   └── src/
│       ├── controllers/    # Route logic (auth, messages)
│       ├── lib/            # DB, Cloudinary, Socket, Utils
│       ├── middleware/     # JWT auth middleware
│       ├── models/         # Mongoose schemas
│       ├── routes/         # API routes
│       └── index.js        # Express server entry point
├── frontend/
│   └── src/
│       ├── components/     # Reusable UI components
│       ├── pages/          # Page views
│       ├── store/          # Zustand state stores
│       ├── lib/            # Axios instance, utils
│       └── App.jsx         # Root component
├── package.json            # Root build & start scripts
├── render.yaml             # Render deployment config
└── README.md
```

---

## 🚀 Getting Started (Local Development)

### Prerequisites
- Node.js >= 18
- MongoDB Atlas account
- Cloudinary account

### 1. Clone the repository
```bash
git clone https://github.com/santhosh-6938/Chat-app.git
cd Chat-app
```

### 2. Set up environment variables
Create a `.env` file inside the `backend/` directory:
```env
MONGODB_URI=your_mongodb_connection_string
PORT=5001
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
NODE_ENV=development
```

### 3. Start the backend
```bash
npm run dev --prefix backend
```

### 4. Start the frontend
```bash
npm run dev --prefix frontend
```

### 5. Open in browser
```
http://localhost:5173
```

---

## ☁️ Deployment

This project is deployed on **Render** as a single unified web service.

The Express backend serves both the REST API and the compiled React frontend in production.

| Setting | Value |
|---|---|
| Build Command | `npm run build` |
| Start Command | `npm start` |
| Environment | `Node` |

---

## 🔑 Environment Variables (Production)

| Variable | Description |
|---|---|
| `MONGODB_URI` | MongoDB Atlas connection string |
| `JWT_SECRET` | Secret key for JWT signing |
| `CLOUDINARY_CLOUD_NAME` | Cloudinary cloud name |
| `CLOUDINARY_API_KEY` | Cloudinary API key |
| `CLOUDINARY_API_SECRET` | Cloudinary API secret |
| `NODE_ENV` | Set to `production` |

---

## 📸 Screenshots

> Sign up, log in, chat in real time, update your profile, and switch themes.

---

## 👤 Author

**Santhosh Bikkina**
- GitHub: [@santhosh-6938](https://github.com/santhosh-6938)

---

## 📄 License

This project is open source and available under the [ISC License](LICENSE).
