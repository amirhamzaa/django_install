# django_install
# Django First Project Setup (Windows)

A beginner-friendly guide documenting the setup of a Django development environment, creating the first project, running the development server, and creating the first application.

## 🛠️ Tech Stack

- **Operating System:** Windows 11
- **Python:** 3.14
- **Django:** 6.0.7
- **Pillow:** 12.3.0
- **Database:** SQLite3

---

## 📦 Step 1: Create a Virtual Environment

```bash
py -m venv .venv
```

Activate the virtual environment:

```bash
.venv\Scripts\activate
```

You should see:

```text
(.venv)
```

---

## 📥 Step 2: Install Django

```bash
pip install django
```

Verify the installation:

```bash
django-admin --version
```

---

## 🖼️ Step 3: Install Pillow

```bash
pip install pillow
```

Pillow is required when working with images in Django applications.

---

## 🚀 Step 4: Create a Django Project

```bash
django-admin startproject firstProject
```

Project structure:

```
firstProject/
│
├── manage.py
└── firstProject/
    ├── __init__.py
    ├── settings.py
    ├── urls.py
    ├── asgi.py
    └── wsgi.py
```

---

## 📂 Step 5: Navigate into the Project

```bash
cd firstProject
```

Check the project files:

```bash
dir
```

---

## ▶️ Step 6: Run the Development Server

Incorrect command:

```bash
py manage .py runserver
```

Correct command:

```bash
py manage.py runserver
```

If successful, Django will display:

```text
Starting development server at http://127.0.0.1:8000/
```

Open your browser and visit:

```
http://127.0.0.1:8000/
```

---

## 🗄️ Step 7: Apply Database Migrations

If Django shows:

```text
You have 18 unapplied migration(s).
```

Run:

```bash
py manage.py migrate
```

This creates the default database tables required by Django.

---

## 📱 Step 8: Create Your First App

```bash
py manage.py startapp core
```

App structure:

```
core/
├── admin.py
├── apps.py
├── migrations/
├── models.py
├── tests.py
└── views.py
```

---

## ⚙️ Step 9: Register the App

Open:

```
firstProject/settings.py
```

Add the app inside `INSTALLED_APPS`:

```python
INSTALLED_APPS = [
    ...
    "core",
]
```

---

## 📁 Project Structure

```
firstProject/
│
├── core/
│   ├── admin.py
│   ├── apps.py
│   ├── migrations/
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── firstProject/
│   ├── settings.py
│   ├── urls.py
│   ├── asgi.py
│   └── wsgi.py
│
├── db.sqlite3
└── manage.py
```

---

## 💻 Useful Django Commands

Create Project

```bash
django-admin startproject firstProject
```

Create App

```bash
py manage.py startapp core
```

Run Server

```bash
py manage.py runserver
```

Create Migrations

```bash
py manage.py makemigrations
```

Apply Migrations

```bash
py manage.py migrate
```

Create Superuser

```bash
py manage.py createsuperuser
```

Open Django Shell

```bash
py manage.py shell
```

Collect Static Files

```bash
py manage.py collectstatic
```

---

## ❗ Common Issues

### Error: `can't open file 'manage'`

Cause:

The command was typed incorrectly.

Correct command:

```bash
py manage.py runserver
```

---

### Warning: `18 unapplied migration(s)`

Run:

```bash
py manage.py migrate
```

---

### Error: `GET /favicon.ico 404`

This is normal.

Browsers automatically request a favicon. Since one has not been added yet, Django returns a 404 response.

---

## 📚 Learning Workflow

```
Create Virtual Environment
        ↓
Activate Environment
        ↓
Install Django
        ↓
Create Project
        ↓
Run Migrations
        ↓
Start Development Server
        ↓
Create App
        ↓
Register App
        ↓
Create Models
        ↓
Create Views
        ↓
Configure URLs
        ↓
Create Templates
        ↓
Build Django Application
```

---

## ✅ Session Summary

- Created a Python virtual environment.
- Activated the virtual environment.
- Installed Django 6.0.7.
- Installed Pillow.
- Created the Django project (`firstProject`).
- Started the Django development server.
- Opened the Django welcome page successfully.
- Created the first app (`core`).
- Learned how to fix a common `manage.py` command error.
- Identified and understood pending database migrations.

---

## 🎯 Next Steps

- Register the `core` app.
- Run migrations.
- Create models.
- Build views.
- Configure URLs.
- Add HTML templates.
- Continue developing your Django application.

---

## 📖 Author

Created while learning **Django Framework**.

Feel free to fork, star ⭐, and contribute!
