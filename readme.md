# 🎓 SmartClass – Full Stack Coursework Project

A full-stack educational course booking system built with **Vue.js, Node.js, Express.js, and MongoDB Atlas using native MongoDB driver (no Mongoose)**.  
This app allows users to browse courses, search, sort, add to cart, remove, and checkout securely.

---

## 🔗 Live Demo & Source Code Links

| Component | Link |
|-----------|------|
| 🌐 GitHub Pages (Frontend Live App) | https://priestlyife.github.io/smartclass-frontend/ |
| 💻 Frontend GitHub Repository | https://github.com/Priestlyife/smartclass-frontend |
| ⚙️ Backend GitHub Repository | https://github.com/Priestlyife/smartclass-backend |
| 🚀 Backend API on Render | https://smartclass-backend-vlj4.onrender.com |

---

## 📌 API Endpoints (Required by Coursework)

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/lessons` | Fetch all lessons from MongoDB |
| POST | `/order` | Save a new order to MongoDB |
| PUT | `/lesson/:id` | Update available spaces for any lesson |

---

## 📦 Technologies Used

### 🔹 Frontend (Vue.js)
- Vue.js (v2)  
- HTML, CSS, JavaScript  
- Fetch API (Promise-based)  
- LocalStorage for Cart  
- Font Awesome icons  
- Hosted on GitHub Pages  

### 🔹 Backend (Node.js, Express.js)
- Express.js (REST API)  
- Native MongoDB Driver (No Mongoose)  
- Logger Middleware (Request logging)  
- Static Image Middleware (optional)  
- Hosted on Render  

### 🔹 Database
- MongoDB Atlas Cloud Database  
  (Collections: `lessons` and `orders`)

---

## ⚙️ Features Implemented (Based on Coursework Requirements)

✔ Display a list of **20 lessons**  
✔ Each lesson includes **title, location, price, availability, and image**  
✔ **Sort** lessons by subject (title), price, location, availability  
✔ **Search** lessons (Frontend-based)  
✔ **Add to cart**, decrease quantity, or remove  
✔ **Checkout page** with validation (Name must be letters, Phone must be numbers)  
✔ **Save Orders to MongoDB** via POST /order  
✔ **Update availability** using PUT /lesson/:id  
✔ Supports **Frontend–Backend Fetch API integration**

---

## 🔧 How to Run Locally

### 1️⃣ Clone the repositories

```bash
git clone https://github.com/Priestlyife/smartclass-backend.git
git clone https://github.com/Priestlyife/smartclass-frontend.git
```

---

### 2️⃣ Install dependencies (Backend only)

```bash
cd smartclass-backend
npm install
```

---

### 3️⃣ Create `.env` file in the backend

```
MONGO_URI=your_atlas_connection_string
PORT=5000
```

---

### 4️⃣ Seed lessons to MongoDB

```bash
node seedCourses.js
```

---

### 5️⃣ Start backend

```bash
npm start
```

---

### 6️⃣ Start frontend

Open `index.html` in `smartclass-frontend` folder or run with a static server (e.g. VS Code Live Server).

---

## 🧪 Testing API with Postman

### 🟢 Get all lessons
```
GET https://smartclass-backend-vlj4.onrender.com/lessons
```

### 🟠 Submit order
```
POST https://smartclass-backend-vlj4.onrender.com/order
```

### 🔵 Update lesson spaces
```
PUT https://smartclass-backend-vlj4.onrender.com/lesson/:id
```

---

## 📁 MongoDB Collections

**lessons (20 records)**  
Fields: `_id`, title, price, location, available, image, instructor, ...

**orders**  
Each document stores: customerName, phone, email, address, items (array), delivery, totalPrice, paymentMethod, createdAt

---

## 📌 Submission Notes

✔ Frontend on GitHub Pages  
✔ Backend hosted on Render.com  
✔ Native MongoDB driver used  
✔ No Mongoose anywhere in backend  
✔ Postman requests prepared  
✔ MongoDB collections exported (via MongoDB Atlas export)  
✔ README includes all required links  

---

## 👨‍💻 Author

**Priestly Akinmulero**  
Software Engineering Student  
Middlesex University  

