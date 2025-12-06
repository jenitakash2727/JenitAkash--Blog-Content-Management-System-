# Blog Content Management System — Django + React

A full-stack Blog CMS built using **Django REST Framework** (Python) and **React.js**, designed for creating, managing, and publishing blog posts with search and filter capabilities.

**Project Creator:** Jenit Akash

---

## 🚀 Features

* ✅ Complete CRUD operations for blog posts
* ✅ Search posts by title, content, or tags
* ✅ Filter posts by category, author, or status
* ✅ Clean Bootstrap-based UI with responsive layout
* ✅ RESTful API with Django backend
* ✅ Simple and intuitive user interface

---

## 🛠️ Technologies Used

* **Backend:** Django, Django REST Framework (Python)
* **Frontend:** React.js, Bootstrap 5
* **Database:** SQLite (development)
* **API Design:** RESTful Architecture
* **Styling:** Bootstrap 5 + Custom CSS

---

## 📂 Project Structure

```
blog-cms/
├── backend/
│   ├── blogapi/        # Django project
│   ├── posts/          # Blog app
│   ├── requirements.txt
│   ├── manage.py
│   └── .env.example
├── frontend/
│   ├── src/
│   │   ├── components/ # Reusable components
│   │   ├── pages/      # Page components
│   │   ├── services/   # API services (axios/fetch wrappers)
│   │   ├── App.jsx
│   │   └── index.js
│   ├── package.json
│   └── .env.example
└── README.md
```

---

## ⚙️ Installation & Setup

> These instructions assume you have `git`, `python` (3.8+), `node` (v16+ or compatible), and `npm` or `yarn` installed.

### 1. Clone the repository

```bash
git clone https://github.com/jenitakash2727/jeevan-tech-blog.git
cd jeevan-tech-blog
```

### 2. Backend (Django) — Setup & Run

```bash
cd backend

# create virtualenv
python -m venv venv

# activate venv
# On Windows:
venv\Scripts\activate
# On macOS / Linux:
# source venv/bin/activate

# install dependencies
pip install -r requirements.txt

# create .env from example and edit if needed
# cp .env.example .env

# apply migrations
python manage.py migrate

# create a superuser (follow prompts)
python manage.py createsuperuser

# run development server
python manage.py runserver
```

The Django API will by default run at `http://127.0.0.1:8000/`.

> TIP: If you want to use a different DB (Postgres/MySQL) update `settings.py` and `.env` accordingly.

### 3. Frontend (React) — Setup & Run

Open a new terminal while backend is running:

```bash
cd frontend

# install dependencies
npm install
# or
# yarn install

# start dev server
npm start
# or
# yarn start
```

React dev server typically runs at `http://localhost:3000/` and will proxy API requests to the backend if proxy is configured in `package.json` or via environment variables.

---

## 🔧 Environment Variables

Use `.env.example` in both `backend/` and `frontend/` as templates. Common backend env variables:

```
SECRET_KEY=your-django-secret-key
DEBUG=True
ALLOWED_HOSTS=localhost,127.0.0.1
DATABASE_URL=sqlite:///db.sqlite3
```

Common frontend env variables (prefix `REACT_APP_`):

```
REACT_APP_API_URL=http://127.0.0.1:8000/api
```

---

## 🧩 API Endpoints (examples)

> Replace `http://127.0.0.1:8000/api/` with your API base URL

* `GET  /api/posts/` — list posts (supports search / filters via query params)
* `POST /api/posts/` — create a post (auth required)
* `GET  /api/posts/{id}/` — retrieve a post
* `PUT  /api/posts/{id}/` — update a post (auth required)
* `DELETE /api/posts/{id}/` — delete a post (auth required)
* `GET  /api/categories/`, `GET /api/tags/`, `GET /api/authors/` — supporting resources

Search & filter example:

```
GET /api/posts/?search=django&category=web&author=3&status=published
```

---

## ✅ Common Development Notes

* Use Django admin (`/admin`) to manage users, categories, tags and quick post edits.
* Protect write endpoints with authentication (e.g., TokenAuth, JWT). Ensure frontend includes auth tokens when calling protected endpoints.
* For production: set `DEBUG=False`, configure `ALLOWED_HOSTS`, use a production-ready DB (Postgres), configure static files & media storage (e.g., S3), and use HTTPS.
* To rebuild the frontend for production:

  ```bash
  cd frontend
  npm run build
  ```

  Copy the `build/` output to your static hosting or serve via Django's staticfiles (or a reverse proxy like nginx).

---

## 🧪 Troubleshooting

* `ModuleNotFoundError` for packages: ensure your venv is activated before `pip install -r requirements.txt`.
* Port conflicts: change `runserver` port (`python manage.py runserver 8001`) or React port (set `PORT=3001` environment var).
* CORS issues: install and configure `django-cors-headers` in backend settings to allow React dev server during development.

---

## 📦 Deployment Checklist (brief)

* Configure environment variables securely
* Use a production web server (Gunicorn + Nginx or similar)
* Use Postgres (or managed DB) instead of SQLite
* Set up static & media storage
* Configure HTTPS (TLS)
* Set up CI/CD (optional) for automated builds and tests

---

## ✍️ Contribution

Contributions are welcome. Fork the repo, create a branch, make changes, and open a PR. Describe changes in the PR and ensure the app runs locally.

---

## 📜 License

This project is MIT licensed — feel free to reuse and improve.

---

## 📬 Contact

Project by **Jenit Akash**.
For questions or collaboration, open an issue or contact via your GitHub profile.

---
