# 📝 Blog Content Management System (CMS)

A full-stack blog CMS application with Django REST API backend and React.js frontend.

## ✨ Features
- ✅ **Complete CRUD Operations** - Create, Read, Update, Delete blog posts
- ✅ **Search Functionality** - Search posts by title, content, or tags
- ✅ **Filtering** - Filter by category, author, or status
- ✅ **Responsive Design** - Works on mobile, tablet, and desktop
- ✅ **RESTful API** - Clean API endpoints following REST principles
- ✅ **User Authentication** (Ready to implement)
- ✅ **Rich Text Editor** (Can be integrated)

## 🛠️ Technology Stack

### **Frontend**
- React.js 18
- React Router DOM
- Axios for API calls
- Bootstrap 5 for styling
- React Hooks

### **Backend**
- Django 4.2
- Django REST Framework
- SQLite (Development)
- CORS headers

### **Tools**
- Git & GitHub
- Postman (API testing)
- VS Code

## 📁 Project Structure

jeevan-tech-blog/
├── backend/ # Django REST API
├── frontend/ # React.js Application
├── docs/ # Documentation
└── README.md # This file




## 🏗️ Installation & Setup

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

# Activate virtual environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env file with your settings

# Run migrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Run development server
python manage.py runserver


cd ../frontend

# Install dependencies
npm install

# Start development server
npm start




Method	Endpoint	Description
GET	/api/posts/	Get all posts
POST	/api/posts/	Create new post
GET	/api/posts/{id}/	Get single post
PUT	/api/posts/{id}/	Update post
DELETE	/api/posts/{id}/	Delete post
GET	/api/posts/?search=query	Search posts
GET	/api/posts/?category=value	Filter by category


Features Implemented
Completed
Create blog posts

Read/View all posts

Update existing posts

Delete posts

Search functionality

Filter by category

Responsive UI

API documentation

Future Enhancements


User authentication

Rich text editor

Image upload

Comment system

Like/Share features

Pagination

Deployment


 Testing the Application
Create a Post:

Navigate to /create

Fill the form and submit

Verify post appears on homepage

Search Posts:

Use search bar to find posts

Test with different keywords

Filter Posts:

Filter by category (Technology, Lifestyle, etc.)

Filter by status (Draft, Published)

Admin Panel:

Visit /admin

Login with superuser credentials

Manage all posts



