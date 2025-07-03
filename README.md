# My-Chat-App (Chatty) - Fullstack Real-Time Chat App

My-Chat-App (also referred to as Chatty) is a full-featured real-time chat application built using the MERN stack (MongoDB, Express, React, Node.js) with TailwindCSS and DaisyUI for clean, responsive UI components. It supports real-time messaging, authentication, and a beautiful, intuitive interface.

---

## 🚀 Live Demo

🔗 [https://my-chat-app-r5t0.onrender.com](https://my-chat-app-r5t0.onrender.com)

---

## 🚀 Features

* 👥 User Authentication (JWT-based login & registration)
* 💬 Real-Time One-to-One Chat
* 📡 Socket.io Integration for live message delivery
* 🌈 Styled using TailwindCSS and DaisyUI
* 🖼️ Clean and responsive UI

---

## 🧠 Tech Stack

### Frontend:

* React
* TailwindCSS
* DaisyUI
* Axios
* Zustand (state management)

### Backend:

* Node.js
* Express.js
* MongoDB (Mongoose ODM)
* Socket.io
* JWT Auth
* dotenv (for env config)

---

## 🛠️ Installation and Setup

### 1. Clone the Repo

```bash
git clone https://github.com/Adree1204/My-Chat-App.git
cd My-Chat-App
```

### 2. Setup Environment Variables

Create a `.env` file inside `backend/` with the following:

```env
PORT=5000
MONGO_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/
JWT_SECRET=your_jwt_secret
```

Create another `.env` file inside `frontend/` with:

```env
VITE_BASE_URL=http://localhost:5000
```

### 3. Install Dependencies & Build

You only need to run:

```bash
npm run build
```

This single command will:

* Install all dependencies in `backend/`
* Install all dependencies in `frontend/`
* Build the frontend app via Vite

✅ No separate `npm install` step is needed because `build` script handles it internally.

---

## 🔄 Running the App (Development Mode)

### Option 1: Run Backend and Frontend Separately

**Backend**

```bash
npm start
```
  OR
  
```bash
cd backend
npm run start
```

**Frontend**

```bash
cd frontend
npm run dev
```

Now open your browser and go to: [http://localhost:5173](http://localhost:5173)

---

### Option 2: Run Both (Fullstack) in One Command

To run both backend and frontend simultaneously, you can add:

```json
"start": "concurrently \"npm run start --prefix backend\" \"npm run dev --prefix frontend\""
```

Install `concurrently` if not already:

```bash
npm install concurrently --save-dev
```

Then just run:

```bash
npm run start
```

✅ This will run:

* `backend` on `localhost:5000`
* `frontend` on `localhost:5173`

All from a **single terminal**.

---

## 🌐 Deployment

> Deployed on **Render**: [https://my-chat-app-r5t0.onrender.com](https://my-chat-app-r5t0.onrender.com)

---

## 📁 Folder Structure

```
My-Chat-App/
├── backend/                   # Node.js + Express API
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── config/
│   ├── middleware/
│   └── .env                   # Backend environment variables
├── frontend/                  # React + Vite + Tailwind + DaisyUI
│   ├── components/
│   ├── pages/
│   ├── store/
│   ├── App.jsx
│   ├── main.jsx
│   └── .env                   # Frontend environment variables
├── package.json               # Root scripts to build and run both ends
├── README.md
```

---

## 💡 Future Enhancements

* Group chats
* Message notifications
* User profile editing
* Message delete/edit support
* Typing indicator

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

---

## 🔥 Created with 💻 and ⚡ by Adree1204
