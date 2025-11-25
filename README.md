🚀 Affiliate Link Management & Payment Platform

A full-stack SaaS-based Affiliate Link Management System that enables creators, marketers, and businesses to generate, categorize, and track affiliate links with real-time analytics, automated payments, and a secure authentication system.
The platform is built for scalability, speed, and ease of use with modern web technologies.

📌 Table of Contents

Features

Tech Stack

Architecture

Installation & Setup

API Endpoints

Future Enhancements

Contributing

License

Contact

🔥 Features
✅ Authentication & Authorization

OAuth 2.0 + Google Login

JWT-based secure session management

RBAC (Role-Based Access Control) with parent–child role hierarchy

🔗 Affiliate Link Management

Create, categorize, and manage affiliate links

Real-time click tracking

UTM-based performance analytics

Expiry & redirect rules

📊 Analytics Dashboard

Real-time charts for clicks, conversions, revenue

Top-performing links

Device/IP tracking (optional)

💰 Automated Payments

Razorpay Integration

Webhook-driven credit flow

Automated wallet update after successful transactions

Subscription plans for users

📂 User & Category Management

Add/manage categories

Multi-user & multi-company support

🛡 Security

Encrypted sensitive data

Secure API endpoints

Input validation + rate limiting

📱 Fully Responsive UI

Modern dashboards

Mobile-friendly layouts

🛠 Tech Stack
Frontend

⚛ React.js

🧰 Redux 

🎨 Tailwind CSS

Backend

🚀 Node.js + Express.js

🗄 MongoDB (Mongoose ORM)

🔗 REST API Architecture

Authentication

🔑 OAuth 2.0 (Google SSO)

🔐 JWT Token Authentication

🛂 RBAC Access Control

Payments

💳 Razorpay + Webhooks

DevOps

🐳 Docker (full app containerization)

🔧 CI/CD (GitHub Actions optional)

🏗 Architecture
Frontend (React + Redux)
        ↓ REST API
Backend (Node.js + Express)
        ↓
Database (MongoDB)
        ↓
Payment Gateway (Razorpay)
        ↓ Webhooks
DevOps (Docker, CI/CD)

⚙ Installation & Setup
📌 Prerequisites

Node.js & npm

MongoDB

Razorpay Keys

Google OAuth Client ID

1️⃣ Clone the Repository
git clone https://github.com/abhinav12222363/Affiliate-Full-Stack-Affiliate-Link-Management-Platform-
cd Affiliate-Full-Stack-Affiliate-Link-Management-Platform-

2️⃣ Install Dependencies
npm install

3️⃣ Create a .env File
MONGO_URI=your_mongo_uri
JWT_SECRET=your_secret
RAZORPAY_KEY_ID=your_key
RAZORPAY_KEY_SECRET=your_secret
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_client_secret

4️⃣ Run the Backend
npm start

5️⃣ Run the Frontend
cd client
npm install
npm start

📡 API Endpoints
Auth Routes
Method	Endpoint	Description
POST	/api/auth/register	Register a new user
POST	/api/auth/login	Login user (JWT)
GET	/api/auth/google	Google OAuth Login
Affiliate Link Routes
Method	Endpoint	Description
POST	/api/link/create	Create new affiliate link
GET	/api/link/all	Get all links
GET	/api/link/:id	Get link details
PUT	/api/link/update/:id	Update link
DELETE	/api/link/delete/:id	Delete link
Payment Routes
Method	Endpoint	Description
POST	/api/pay/order	Create payment order
POST	/api/pay/webhook	Razorpay webhook listener
🚀 Future Enhancements

📌 Multi-currency support

📱 Mobile App (React Native)

🧠 AI-based link performance prediction

🎯 Affiliate marketplace system

📊 Exportable PDF reports

💼 Team collaboration features

🤝 Contributing

Contributions are welcome!
Feel free to fork the repo, create a branch, and submit a pull request.

📜 License

This project is licensed under the MIT License.

📬 Contact

Abhinav Prakash
📧 Email: abhinavkumar8789@gmail.com

🌐 GitHub: https://github.com/abhinav12222363

🔗 Project Link:
https://github.com/abhinav12222363/Affiliate-Full-Stack-Affiliate-Link-Management-Platform-
