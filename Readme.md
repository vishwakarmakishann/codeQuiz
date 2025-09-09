# 📚 CodeQuiz

A full-stack web application for creating, managing, and taking quizzes.  
It supports **admin functionalities** (quiz & question management) and **user functionalities** (register, take quizzes, and view results).

---

## 🚀 Features

### 👤 User
- Register & Login
- Browse available quizzes
- Attempt quizzes with multiple-choice questions
- Instant result & explanation display

### 🛠️ Admin
- Create, edit, and delete quizzes
- Add, edit, and delete questions
- View all quizzes and manage users

---


## ⚙️ Tech Stack

**Frontend**
- React + Vite
- TailwindCSS
- React Router

**Backend**
- Node.js
- Express.js
- MongoDB + Mongoose
- express-session

---

## 📸 ScreenShots

**Landing page**
![alt text](Frontend/src/assets/screenshots/landing.png)

**Login**
![alt text](Frontend/src/assets/screenshots/login.png)

**Quiz selection**
![alt text](Frontend/src/assets/screenshots/quizSelection.png)

**Question**
![alt text](Frontend/src/assets/screenshots/question.png)

**Result**
![alt text](Frontend/src/assets/screenshots/result.png)

**Admin**
![alt text](Frontend/src/assets/screenshots/admin.png)

**View Quizzes**
![alt text](Frontend/src/assets/screenshots/viewQuiz.png)

**View Questions**
![alt text](Frontend/src/assets/screenshots/viewUser.png)

---

## 🔧 Installation & Setup

```bash
1️⃣ Clone the repository
git clone https://github.com/your-username/codeQuiz.git
cd codeQuiz

2️⃣ Backend Setup

cd Backend
npm install

Create a .env file:
PORT=4000
MONGO_URI=your_mongodb_connection

Start backend server:
node app.js

3️⃣ Frontend Setup
cd ../Frontend
npm install

Start frontend:
npm run dev


```

## 📌 API Endpoints
**Authentication**
- POST /auth/register → Register user
- POST /auth/login → Login user
- POST /auth/logout → Logout user

**Quizzes**
- POST /quiz → Create new quiz (Admin)
- PATCH /quiz/:id → Edit quiz (Admin)
- DELETE /quiz/:id → Delete quiz (Admin)
- GET /quiz → Get all quizzes
- GET /quiz/:id → Get all quiz

**Questions**
- POST /question → Add question (Admin)
- PATCH /question/:id → Edit question (Admin)
- DELETE /question/:id → Delete question (Admin)
- GET /question/:id → Get question
- GET /question/quiz/:id → Get questions for a quiz
- GET /question → Get all questions