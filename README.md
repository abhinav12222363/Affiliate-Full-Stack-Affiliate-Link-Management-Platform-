# 🚀 Affiliate Link Management & Payment Platform

A full-stack SaaS-based **Affiliate Link Management System** that enables creators, marketers, and businesses to generate, categorize, and track affiliate links with real-time analytics, automated payments, and secure authentication.

The platform is built for **scalability**, **speed**, and **ease of use**, powered by modern web technologies and production-ready containerization.

---

## 📌 Table of Contents

- Features
- Tech Stack
- Architecture
- Installation (Local)
- Installation (Docker)
- Environment Variables
- API Endpoints
- Future Enhancements
- Contributing
- License
- Contact

---

## 🔥 Features

### ✅ Authentication & Authorization
- OAuth 2.0 (Google Login)
- JWT-based session security
- RBAC (Role-Based Access Control)
- Pagination

### 🔗 Affiliate Link Management
- Create & manage affiliate links
- Real-time click tracking
- UTM analytics
- Expiry & redirect rules

### 📊 Analytics Dashboard
- Clicks, conversions, revenue
- Top performing links
- Device & IP tracking (optional)

### 💰 Automated Payments
- Razorpay integration
- Webhook-based order handling
- Auto wallet updates
- Subscription plans

### 📂 User & Category Management
- Category-based link organization
- Multi-user & multi-company support

### 🛡 Security
- Encrypted sensitive data
- Secure API routes
- Input validation + rate limiting

### 📱 Fully Responsive UI
- Modern dashboards
- Mobile-ready layouts

---

## 🛠 Tech Stack

### Frontend
- ⚛ React.js
- 🧰 Redux Toolkit
- 🎨 Tailwind CSS / Material UI

### Backend
- 🚀 Node.js + Express.js
- 🗄 MongoDB (Mongoose ORM)
- 🔗 REST API

### Authentication
- 🔑 Google OAuth 2.0
- 🔐 JWT auth
- 🛂 RBAC access control

### Payments
- 💳 Razorpay + Webhooks

### DevOps
- 🐳 Docker (Full containerization)
- 🔧 CI/CD (GitHub Actions Ready)

---

## 🏗 Architecture

Frontend (React + Redux)
↓ REST API
Backend (Node.js + Express)
↓
Database (MongoDB Atlas)
↓
Payment Gateway (Razorpay)
↓ Webhooks
DevOps (Docker, CI/CD)


---

# ⚙ Installation & Setup (Local Development)

### 📌 Prerequisites
- Node.js & npm
- MongoDB (Cloud or Local)
- Razorpay Keys
- Google OAuth Client ID

### 1️⃣ Clone Repository
```sh
git clone https://github.com/abhinav12222363/Affiliate-Full-Stack-Affiliate-Link-Management-Platform-.git
cd Affiliate-Full-Stack-Affiliate-Link-Management-Platform-

2️⃣ Install Backend Dependencies
npm install

3️⃣ Configure Environment File

Create .env in /server:

PORT=5001
MONGO_URI=your_mongo_uri
JWT_SECRET=your_secret
CLIENT_URL=http://localhost:3000
RAZORPAY_KEY_ID=your_key
RAZORPAY_KEY_SECRET=your_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

4️⃣ Run Backend
npm start

5️⃣ Run Frontend
cd client
npm install
npm start

🐳 Docker Setup (Production Recommended)
📌 Prerequisites

Docker

Docker Compose (optional)

1️⃣ Backend Docker Image
docker build -t affiliate-backend ./server
docker run -p 5001:5001 --env-file ./server/.env affiliate-backend

2️⃣ Frontend Docker Image
docker build -t affiliate-frontend ./client
docker run -p 3000:80 affiliate-frontend

🐳 Docker Compose Setup (Full Stack)

Create docker-compose.yml:

version: "3.9"
services:
  backend:
    build: ./server
    ports:
      - "5001:5001"
    env_file:
      - ./server/.env
    depends_on:
      - mongo

  frontend:
    build: ./client
    ports:
      - "3000:80"
    depends_on:
      - backend

  mongo:
    image: mongo:6
    restart: always
    ports:
      - "27017:27017"


Run full stack:

docker compose up --build -d

📡 API Endpoints
Auth Routes
Method	Endpoint	Description
POST	/api/auth/login	Login user
POST	/api/auth/register	Register
GET	/api/auth/google	Google OAuth
Affiliate Link Routes
Method	Endpoint	Description
POST	/api/link/create	Create new link
GET	/api/link/all	Get all links
GET	/api/link/:id	Get link details
PUT	/api/link/update/:id	Update link
DELETE	/api/link/delete/:id	Delete link
Payment Routes
Method	Endpoint	Description
POST	/api/pay/order	Create Razorpay order
POST	/api/pay/webhook	Payment webhook
🚀 Future Enhancements

📌 Multi-currency support

📱 Mobile App (React Native)

🧠 AI performance predictions

🎯 Affiliate marketplace system

📊 Exportable PDF reports

💼 Team collaboration features

🤝 Contributing

Contributions are welcome!
Feel free to fork, create a branch, and submit a PR.

📜 License

This project is licensed under the MIT License.

📬 Contact

Abhinav Prakash

📧 Email: abhinavkumar8789@gmail.com
🌐 GitHub: https://github.com/abhinav12222363

🔗 Project Link: https://github.com/abhinav12222363/Affiliate-Full-Stack-Affiliate-Link-Management-Platform-
