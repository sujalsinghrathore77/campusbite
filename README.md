<div align="center">

<img src="assets/logo.png" alt="CampusBite Logo" width="180"/>

# 🍽️ CampusBite

### Smart College Canteen Token System

Digitizing campus dining with **online ordering, digital tokens, QR payments, and real-time order tracking**.

[🌐 Landing Page](https://campusbiteait.netlify.app) •
[🚀 Live Demo](https://campusbite-peach.vercel.app/) •
[💻 GitHub Repository](https://github.com/sujalsinghrathore77/campusbite)

## 🚀 Demo Access

### Student Demo

Email: student@acharya.ac.in

Password: ********
</div>

---

# 📖 Overview

CampusBite is a modern **College Canteen Management System** designed to eliminate long queues and simplify food ordering inside college campuses.

Students can browse menus, place orders, pay online or at the counter, receive a digital token, and track their order in real time.

The platform also provides dedicated dashboards for canteen staff and administrators to efficiently manage menus, payments, and incoming orders.

---

# ✨ Features

## 👨‍🎓 Student

- Secure college email authentication
- Browse multiple canteens
- Search & filter menu items
- Add items to cart
- Online UPI QR or counter payment
- Digital token generation
- Real-time order tracking
- Responsive mobile interface

---

## 👨‍🍳 Canteen Dashboard

- Receive incoming orders
- Update order status
- Manage menu availability
- View daily statistics
- Complete or cancel orders

---

## 👨‍💼 Admin Dashboard

- Manage canteens
- Manage menu items
- Upload & manage QR payments
- Revenue overview
- Category management
- Staff management

---

# 🛠 Tech Stack

| Category | Technology |
|-----------|------------|
| Frontend | React 18, Tailwind CSS, shadcn/ui |
| Backend | FastAPI (Python) |
| Database | MongoDB |
| Authentication | JWT + Supabase Auth |
| Payments | UPI QR Integration |
| Deployment | Vercel, Railway, Netlify |

---

# 📱 Application Preview

## 🏠 Landing Page

The landing page introduces CampusBite and allows users to access the food ordering platform.

![Landing Page](screenshots/1-landing-page.png)

---

## 🔐 Login / Register

Students securely register and log in using their official college email address.

![Login](screenshots/2-login.png)

---

## 🍽️ Student Menu

Browse food items from multiple canteens, search meals, filter categories, and add items to the cart.

![Student Menu](screenshots/3-student-menu.png)

---

## 🛒 Cart & Checkout

Review selected items, update quantities, and verify the order before checkout.

![Cart](screenshots/4-cart.png)

---

## 💳 QR Payment

Students can pay online using a dynamic UPI QR code or choose to pay at the counter.

![Payment](screenshots/5-payment.png)

---

## 🎟 Order Tracking

Track every order from **Pending → Preparing → Completed** using a digital token.

![Order Tracking](screenshots/6-order-tracking.png)

---

## 👨‍🍳 Canteen Dashboard

Canteen staff can manage orders through an easy-to-use dashboard with live status updates.

![Canteen Dashboard](screenshots/7-canteen-dashboard.png)

---

## 👨‍💼 Admin Dashboard

The admin dashboard provides centralized control over canteens, menus, payments, and analytics.

![Admin Dashboard](screenshots/8-admin-dashboard.png)

---

# 🔄 Order Flow

```text
Student Login
      │
      ▼
Browse Menu
      │
      ▼
Add to Cart
      │
      ▼
Checkout
      │
      ▼
UPI / Counter Payment
      │
      ▼
Digital Token Generated
      │
      ▼
Kitchen Receives Order
      │
      ▼
Preparing
      │
      ▼
Completed
      │
      ▼
Collect Food
```

---# 🚀 Local Development

## Prerequisites

Make sure you have the following installed:

- Node.js 18+
- Python 3.9+
- MongoDB
- Git

---

## Clone Repository

```bash
git clone https://github.com/sujalsinghrathore77/campusbite.git
cd campusbite
```

---

## Frontend Setup

```bash
cd frontend
npm install
npm start
```

The frontend will be available at:

```
http://localhost:3000
```

---

## Backend Setup

```bash
cd backend

pip install -r requirements.txt

uvicorn server:app --reload --port 8001
```

The backend API will run at:

```
http://localhost:8001
```

---

# ☁️ Deployment

CampusBite is deployed using the following services:

| Component | Platform |
|-----------|----------|
| Frontend | Vercel |
| Backend | Railway |
| Landing Page | Netlify |
| Database | MongoDB |

---

## Frontend Deployment (Vercel)

1. Push your repository to GitHub.
2. Import the repository into Vercel.
3. Configure:

```
Build Command:
npm run build

Output Directory:
build

Install Command:
npm install
```

4. Add the required environment variable:

```
REACT_APP_BACKEND_URL
```

---

## Backend Deployment

Deploy the FastAPI backend to any Python-supported hosting platform.

Recommended platforms:

- Railway ✅
- Render
- Fly.io
- AWS
- Google Cloud

Required Environment Variables:

```
MONGO_URL
DB_NAME
JWT_SECRET
CORS_ORIGINS
```

---

# 🔐 Environment Variables

## Frontend (`frontend/.env`)

```env
REACT_APP_BACKEND_URL=https://your-backend-url.com

REACT_APP_SUPABASE_URL=https://your-project.supabase.co

REACT_APP_SUPABASE_ANON_KEY=your-supabase-anon-key
```

---

## Backend (`backend/.env`)

```env
MONGO_URL=mongodb://localhost:27017

DB_NAME=campusbite

JWT_SECRET=your-secret-key

CORS_ORIGINS=https://your-frontend-url.com

ADMIN_EMAIL=admin@example.com

ADMIN_PASSWORD=your-strong-admin-password

# Supabase

SUPABASE_URL=https://your-project.supabase.co

SUPABASE_SERVICE_ROLE_KEY=your-service-role-key

SUPABASE_JWT_SECRET=your-jwt-secret

ALLOWED_EMAIL_DOMAIN=acharya.ac.in

ALLOW_LEGACY_STUDENT_LOGIN=false
```

---

# 📂 Project Structure

```
CampusBite
│
├── frontend
│   ├── public
│   ├── src
│   │   ├── components
│   │   ├── contexts
│   │   ├── pages
│   │   ├── hooks
│   │   ├── lib
│   │   └── assets
│   │
│   └── package.json
│
├── backend
│   ├── server.py
│   ├── requirements.txt
│   └── routes
│
├── assets
│   └── logo.png
│
├── screenshots
│   ├── 1-landing-page.png
│   ├── 2-login.png
│   ├── 3-student-menu.png
│   ├── 4-cart.png
│   ├── 5-payment.png
│   ├── 6-order-tracking.png
│   ├── 7-canteen-dashboard.png
│   └── 8-admin-dashboard.png
│
├── README.md
└── vercel.json
```

---

# 🏗️ Build for Production

## Frontend

```bash
cd frontend

npm run build
```

Production build output:

```
frontend/build/
```

---

## Backend

Run the FastAPI application using:

```bash
uvicorn server:app --host 0.0.0.0 --port 8001
```

For production deployments, consider using:

- Gunicorn + Uvicorn Workers
- Railway
- Docker
- Nginx (Reverse Proxy)# 🔑 Supabase Authentication

CampusBite uses **Supabase Authentication** to securely manage student accounts.

Only users with an authorized college email domain can register and access the platform.

Example:

```
student@acharya.ac.in
```

For the complete authentication setup, database schema, SQL scripts, and environment configuration, refer to:

```
SUPABASE_SETUP.md
```

---

# 🤝 Contributing

Contributions are always welcome!

If you'd like to improve CampusBite, follow these steps:

1. Fork the repository
2. Create a new feature branch

```bash
git checkout -b feature/your-feature
```

3. Commit your changes

```bash
git commit -m "Add new feature"
```

4. Push your branch

```bash
git push origin feature/your-feature
```

5. Open a Pull Request

Please make sure your code follows the existing project structure and coding style.

---

# 📄 License

This project is licensed under the **MIT License**.

Feel free to use, modify, and distribute it under the terms of the license.

---

# 👨‍💻 Author

## Sujal Singh Rathore

Information Science Engineering Student

Acharya Institute of Technology

### Connect with me

- GitHub: https://github.com/sujalsinghrathore77
- X (Twitter): https://x.com/SujalSRathore
- LinkedIn: https://www.linkedin.com/in/sujal-singh-rathore-432b4b30b?utm_source=share_via&utm_content=profile&utm_medium=member_android

---

# 🌟 Support

If you found this project useful,

⭐ Star the repository

🍴 Fork it

🛠️ Contribute

💬 Share your feedback

Every contribution and suggestion helps make CampusBite better.

---

<div align="center">

Made with ❤️ by **Sujal Singh Rathore**

</div>
