# 🛒 E-Commerce Backend

A scalable backend API powering a full-stack e-commerce application. Built with **Node.js**, **Express**, and **MongoDB**, this backend provides secure user authentication, product management, cart operations, and order processing.

---

## 🚀 Tech Stack

- **Backend Framework**: Node.js, Express.js
- **Database**: MongoDB (Mongoose ODM)
- **Authentication**: JWT (JSON Web Token)
- **Password Encryption**: bcrypt
- **Middleware**: Custom middlewares for error handling and auth
- **Environment Config**: dotenv
- **Deployment**: Render backend (depending on your deployment)

---

## 🎯 Features

- ✅ **User Authentication**
  - Register, Login, Secure JWT sessions
  - Password hashing with bcrypt
- ✅ **Product Management**
  - Add, update, delete, and list products
- ✅ **Cart Management**
  - Add/remove items to user cart


  🏃‍♂️ Getting Started
1️⃣ Clone the repository
```
git clone https://github.com/gopalkrs/ecommerce-backend.git
cd ecommerce-backend
```
2️⃣ Install dependencies
```
npm install
```
3️⃣ Setup environment variables
Create a .env file in the root directory with:
```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
```
4️⃣ Start the server
```
npm run dev
The backend server will run on http://localhost:5000.
```

🛠 Sample API Endpoints
User Routes
POST /api/auth/register - Register new user

POST /api/auth/login - User login

GET /api/user/profile - Get user profile (protected)

Product Routes
POST /api/products/ - Create new product (admin only)

GET /api/products/ - Get all products

GET /api/products/:id - Get product details

Cart Routes
POST /api/cart/add - Add product to cart

DELETE /api/cart/remove/:productId - Remove product from cart

Order Routes
POST /api/orders/ - Place order

GET /api/orders/:id - Get order details

🔒 Security Practices
Passwords encrypted using bcrypt

JWT-based stateless authentication

Secure API design using middlewares

Input validation with Zod


