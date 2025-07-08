
# Order Management Web App

A full-stack backend project built using **Node.js**, **Express**, and **MongoDB**, designed to handle users, customers, and order workflows. The system supports RESTful APIs, user authentication, and scalable CRUD operations using an MVC architecture.

## 🧠 Objective

To develop a modular backend system that enables order management functionalities including user login, customer record handling, and order data tracking — with support for secure API endpoints and role-based access control.

---

## 🏗️ Features

- ✅ REST APIs for:
  - User registration and login (JWT-based)
  - Customer data management
  - Order creation, update, and deletion
  - File uploads (using `multer`)
- ✅ Follows **MVC** architecture
- ✅ MongoDB models for `User`, `Customer`, and `Order`
- ✅ Middleware for authentication, error handling, and request validation
- ✅ CORS and JSON parsing enabled for frontend integration

---

## 🧱 Tech Stack

| Layer        | Tech                         |
|--------------|------------------------------|
| Runtime      | Node.js                      |
| Framework    | Express.js                   |
| Database     | MongoDB + Mongoose ODM       |
| Auth         | JWT (JSON Web Token)         |
| File Uploads | Multer                       |
| Versioning   | Git                          |
| Tools        | Postman, MongoDB Compass     |

---

## 🗂️ Project Structure

```
server/
│
├── controllers/       # Business logic for routes
├── models/            # Mongoose schemas
├── routes/            # All route definitions
├── middleware/        # Auth, error handling, etc.
├── uploads/           # Uploaded files
├── index.js           # Main entry point
└── package.json
```

---

## ⚙️ Setup & Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/order-management-app.git
   cd order-management-app/server
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Create `.env` file**
   ```
   MONGO_URI=<your-mongodb-uri>
   JWT_SECRET=<your-secret>
   ```

4. **Run the server**
   ```bash
   npm start
   ```

---

## 🔒 API Authentication

All protected routes require a `Bearer` token passed in the `Authorization` header. Tokens are issued during user login or registration.

---

## 📬 API Endpoints (Examples)

- `POST /api/auth/signup` – Register user  
- `POST /api/auth/login` – Login and receive token  
- `GET /api/customer/` – List customers (protected)  
- `POST /api/order/` – Create new order (protected)

---

## 📌 Future Improvements

- Add frontend (React or Vue)  
- Integrate email notification system  
- Add dashboard analytics  
- Role-based access (admin, staff, etc.)

---

## 📄 License

This is a self project created for learning and demonstration purposes. Feel free to fork and build upon it.
