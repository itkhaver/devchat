
# 💬 DevChat - A Chat App for Developers by Developers

DevChat is a modern, real-time chat application built specifically for developers. It focuses on providing a distraction-free, secure, and fast messaging environment. Think of it as "WhatsApp meets GitHub" — built with developers in mind, offering minimal clutter and maximum performance.

> 🔗 Live preview (coming soon): [https://devchat.itkhaver.com](https://devchat.itkhaver.com)

---

## ✨ Features (Completed So Far)

- 🧑‍💻 **Authentication System**
  - Sign up with username & password (no email required)
  - Secure password hashing using bcrypt
  - Persistent login sessions using JWT tokens
  - Auth state stored in localStorage for auto login on refresh

- 💬 **Chat Interface**
  - Modern, dark-themed UI using TailwindCSS
  - Sidebar with user list and online/offline status indicators
  - Responsive layout inspired by WhatsApp Web
  - Real-time chat logic in progress

- ⚙️ **Settings Panel**
  - Update username and password
  - Logout functionality
  - Clean modal-based or sidebar-based design (WIP)

- 🧑‍🤝‍🧑 **About Page**
  - Fully designed About section with AOS animation
  - Introduces DevChat’s mission and community focus
  - Displays stats (users, uptime, global access)

- 🌐 **Responsive Navigation**
  - Mobile-first design
  - Hamburger menu for mobile view
  - AOS-powered transitions for smooth page experience

- 🎨 **UI & Animation**
  - Tailwind CSS for styling
  - AOS (Animate On Scroll) for smooth UI animations

---

## 🧠 Tech Stack

### 🔗 Frontend
- **React.js** – SPA architecture, component-based UI
- **Tailwind CSS** – Utility-first styling
- **AOS** – Scroll animations
- **React Router** (WIP) – For client-side routing between pages

### 🧩 Backend
- **Node.js** – Server-side runtime
- **Express.js** – RESTful API framework
- **MongoDB** – NoSQL database for storing users and chats
- **Mongoose** – ODM for MongoDB
- **bcrypt.js** – Secure password hashing
- **jsonwebtoken** – Auth token generation and verification
- **CORS + dotenv** – Config and security essentials

---

## 📁 Project Structure (Frontend)

```bash
/public
  └── index.html
/src
  ├── components/
  │   ├── Footer.jsx
  │   ├── Navbar.jsx
  │   ├── ProtectedRoute.jsx
  ├── pages/
  │   ├── Home.jsx
  │   ├── About.jsx
  │   ├── Login.jsx
  │   ├── Register.jsx
  │   ├── Chat.jsx
  │   ├── Settings.jsx
  ├── App.jsx
  ├── main.jsx
```

---

## 🛠 Backend Structure

```bash
/server
  ├── models/
  │   └── User.js
  │   └── Message.js
  ├── routes/
  │   ├── auth.js
  │   ├── users.js
  ├── controllers/
  │   ├── authController.js
  │   ├── chatController.js
  ├── middleware/
  │   └── authMiddleware.js
  ├── routes/
  │   ├── authRoutes.js
  │   ├── chatRoutes.js
  ├── config/
  │   └── db.js
  ├── socket/
  │   └── chatSocket.js
  └── server.js
```

---

## 🚀 Getting Started

### 🖥 Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

### ⚙️ Backend Setup
```bash
cd backend
npm install
node server.js
```

Make sure to add your `.env` file with:
```
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

---

## 🌍 Hosted On
- 🔗 Subdomain: [devchat.itkhaver.com](https://devchat.itkhaver.com)


---

## 👨‍💻 Built With ❤️ by IT-Khaver
[IT-Khaver](https://itkhaver.com) – *"Digital Transform Hub"*

---

## 📅 Roadmap

- [x] Authentication (username & password only)
- [x] UI: Chat page, About page, Features page
- [x] Online/offline status
- [ ] Real-time messaging with socket.io
- [ ] Group chat support
- [ ] Message history persistence
- [ ] Typing indicators
- [ ] Code snippet sharing
- [ ] Theme customizer (light/dark toggle)
