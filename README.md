# 📝 Blog Content Management System (CMS)

A full-stack blog CMS application with Django REST API backend and React.js frontend.

## 🚀 Live Demo
- **Frontend:** [Live URL] (Vercel/Netlify)
- **Backend API:** [API URL] (Render/Railway)
- **Admin Panel:** [Admin URL]
- **API Documentation:** [Postman/Swagger]

## 🎯 Project Overview
This project is a complete Blog Management System that allows users to create, read, update, and delete blog posts. It includes search, filter functionalities and a responsive UI.

## 🏗️ Project Structure

### **Frontend** (`/frontend`)
- **Technology:** React.js 18
- **State Management:** React Hooks
- **Styling:** Bootstrap 5 + Custom CSS
- **Routing:** React Router DOM v6
- **API Calls:** Axios

### **Backend** (`/backend`)
- **Framework:** Django 4.2 + Django REST Framework
- **Database:** SQLite (Development) / PostgreSQL (Production ready)
- **Authentication:** Ready to implement
- **API Design:** RESTful architecture

## ✨ Features

### ✅ Implemented
- **CRUD Operations:** Create, Read, Update, Delete blog posts
- **Search:** Search posts by title, content, or tags
- **Filter:** Filter by category, author, or status
- **Responsive Design:** Mobile-first approach
- **REST API:** Clean API endpoints
- **Form Validation:** Client-side validation

### 🔄 Planned
- User Authentication & Authorization
- Rich Text Editor
- Image Upload
- Comment System
- Pagination
- Social Sharing

## 📸 Screenshots

| Page | Screenshot |
|------|------------|
| **Home Page** | ![Home](screenshots/home.png) |
| **Create Post** | ![Create](screenshots/create.png) |
| **Post List** | ![List](screenshots/list.png) |
| **Admin Panel** | ![Admin](screenshots/admin.png) |

## 🛠️ Technology Stack

### **Frontend**
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Bootstrap](https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

### **Backend**
![Django](https://img.shields.io/badge/Django-092E20?style=for-the-badge&logo=django&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![REST API](https://img.shields.io/badge/REST_API-02569B?style=for-the-badge&logo=google-cloud&logoColor=white)

## 🏁 Getting Started

### **Prerequisites**
- Python 3.8+
- Node.js 16+
- Git

### **Backend Setup**
```bash
# Clone repository
git clone https://github.com/jenitakash2727/jeevan-tech-blog.git
cd jeevan-tech-blog/backend

# Create virtual environment
python -m venv venv

# Activate (Windows)
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Setup environment
cp .env.example .env
# Edit .env with your settings

# Run migrations
python manage.py migrate

# Create admin user
python manage.py createsuperuser

# Run server
python manage.py runserver

