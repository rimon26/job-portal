# 🌐 Job Portal - Next.js | Firebase | MySQL

![Project Banner](https://via.placeholder.com/1200x300?text=Job+Portal+Project+Banner)

A modern, real-time **Job Portal** web application built with **Next.js**, **Firebase Authentication**, and **MySQL**.  
Users can browse jobs, apply, and manage applications seamlessly.

---

## 🚀 Live Demo

[![Live Demo](https://img.shields.io/badge/View-Live-DodgerBlue?style=for-the-badge&logo=vercel)](https://your-live-demo-link.com)

---

## 🎯 Features

- 🔑 **Firebase Authentication** (Sign Up, Login, Logout)
- 📋 **Job Listings** with real-time updates
- ✍️ **Apply for Jobs** & track applications
- 👨‍💻 **Admin Panel** to manage jobs & users
- 🔍 **Search & Filter Jobs** (category, location, keywords)
- 📱 **Responsive Design** (mobile + desktop)
- 🌗 **Dark & Light Mode** toggle

---

## 🛠️ Tech Stack

| Layer          | Technology                                 |
| -------------- | ------------------------------------------ |
| Frontend       | Next.js, React, Tailwind CSS / CSS Modules |
| Backend        | Node.js, Express.js                        |
| Database       | MySQL                                      |
| Authentication | Firebase Auth                              |
| Hosting        | Vercel / Firebase Hosting                  |
| Real-time Data | Firebase Firestore (optional)              |

![Tech Stack](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs)
![Tech Stack](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase)
![Tech Stack](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql)
![Tech Stack](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react)
![Tech Stack](https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwind-css)

---

## 📸 Screenshots

![Landing Page](https://via.placeholder.com/800x400?text=Landing+Page)
![Job Listings](https://via.placeholder.com/800x400?text=Job+Listings)
![Admin Panel](https://via.placeholder.com/800x400?text=Admin+Panel)

---

## 🏗️ Getting Started (All-in-One)

Follow these steps to run the Job Portal project locally. Copy everything into your terminal or editor.

# 1️⃣ Clone the repository

```bash
git clone https://github.com/<your-username>/<repo-name>.git
cd <repo-name>
```

## 2️⃣ Install dependencies

```bash
npm install
# or
yarn install
```

## 3️⃣ Create .env.local file (replace placeholders with your own values)

```bash
echo "NEXT_PUBLIC_FIREBASE_API_KEY=your_api_key
NEXT_PUBLIC_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
NEXT_PUBLIC_FIREBASE_PROJECT_ID=your_project_id
NEXT_PUBLIC_FIREBASE_STORAGE_BUCKET=your_bucket
NEXT_PUBLIC_FIREBASE_MESSAGING_SENDER_ID=your_sender_id
NEXT_PUBLIC_FIREBASE_APP_ID=your_app_id
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=job_portal" > .env.local
```

## 4️⃣ Set up MySQL database and tables

```bash
mysql -u root -p -e "CREATE DATABASE IF NOT EXISTS job_portal;
USE job_portal;

CREATE TABLE IF NOT EXISTS users (
  id INT AUTO_INCREMENT PRIMARY KEY,
  name VARCHAR(255),
  email VARCHAR(255) UNIQUE,
  role ENUM('user', 'admin') DEFAULT 'user'
);

CREATE TABLE IF NOT EXISTS jobs (
  id INT AUTO_INCREMENT PRIMARY KEY,
  title VARCHAR(255),
  description TEXT,
  location VARCHAR(255),
  company VARCHAR(255),
  created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);"
```

## 5️⃣ Run the development server

```bash
npm run dev
# or
yarn dev
```

## ✅ Open your browser at http://localhost:3000
