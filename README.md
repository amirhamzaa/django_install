# django_install

--->
Microsoft Windows [Version 10.0.22000.2538]
(c) Microsoft Corporation. All rights reserved.

D:\py>py -m venv .venv

D:\py>.venv\Scripts\activate

(.venv) D:\py>pip install django
Collecting django
  Downloading django-6.0.7-py3-none-any.whl.metadata (3.9 kB)
Collecting asgiref>=3.9.1 (from django)
  Downloading asgiref-3.12.1-py3-none-any.whl.metadata (9.4 kB)
Collecting sqlparse>=0.5.0 (from django)
  Downloading sqlparse-0.5.5-py3-none-any.whl.metadata (4.7 kB)
Collecting tzdata (from django)
  Downloading tzdata-2026.3-py2.py3-none-any.whl.metadata (1.4 kB)
Downloading django-6.0.7-py3-none-any.whl (8.4 MB)
   ---------------------------------------- 8.4/8.4 MB 9.1 MB/s  0:00:00
Downloading asgiref-3.12.1-py3-none-any.whl (25 kB)
Downloading sqlparse-0.5.5-py3-none-any.whl (46 kB)
Downloading tzdata-2026.3-py2.py3-none-any.whl (348 kB)
Installing collected packages: tzdata, sqlparse, asgiref, django
Successfully installed asgiref-3.12.1 django-6.0.7 sqlparse-0.5.5 tzdata-2026.3

(.venv) D:\py>pip install pillow
Collecting pillow
  Downloading pillow-12.3.0-cp314-cp314-win_amd64.whl.metadata (9.3 kB)
Downloading pillow-12.3.0-cp314-cp314-win_amd64.whl (7.2 MB)
   ---------------------------------------- 7.2/7.2 MB 28.5 MB/s  0:00:00
Installing collected packages: pillow
Successfully installed pillow-12.3.0

(.venv) D:\py>django-admin startproject firstProject

(.venv) D:\py>cd firstProject

(.venv) D:\py\firstProject>dir
 Volume in drive D is New Volume
 Volume Serial Number is ACB5-9DE6

 Directory of D:\py\firstProject

07/26/2026  07:07 PM    <DIR>          .
07/26/2026  07:07 PM    <DIR>          ..
07/26/2026  07:07 PM    <DIR>          firstProject
07/26/2026  07:07 PM               690 manage.py
               1 File(s)            690 bytes
               3 Dir(s)   2,664,509,440 bytes free

(.venv) D:\py\firstProject>py manage .py runserver
D:\py\.venv\Scripts\python.exe: can't open file 'D:\\py\\firstProject\\manage': [Errno 2] No such file or directory

(.venv) D:\py\firstProject>py manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).

You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.
July 26, 2026 - 19:20:20
Django version 6.0.7, using settings 'firstProject.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.

WARNING: This is a development server. Do not use it in a production setting. Use a production WSGI or ASGI server instead.
For more information on production servers see: https://docs.djangoproject.com/en/6.0/howto/deployment/

(.venv) D:\py\firstProject>

(.venv) D:\py\firstProject>

(.venv) D:\py\firstProject>py manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).

You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.
July 26, 2026 - 19:23:50
Django version 6.0.7, using settings 'firstProject.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.

WARNING: This is a development server. Do not use it in a production setting. Use a production WSGI or ASGI server instead.
For more information on production servers see: https://docs.djangoproject.com/en/6.0/howto/deployment/
[26/Jul/2026 19:24:02] "GET / HTTP/1.1" 200 12068
Not Found: /favicon.ico
[26/Jul/2026 19:24:17] "GET /favicon.ico HTTP/1.1" 404 2214

(.venv) D:\py\firstProject>
(.venv) D:\py\firstProject>
(.venv) D:\py\firstProject>py manage.py startapp core

(.venv) D:\py\firstProject>dir
 Volume in drive D is New Volume
 Volume Serial Number is ACB5-9DE6

 Directory of D:\py\firstProject

07/26/2026  07:26 PM    <DIR>          .
07/26/2026  07:07 PM    <DIR>          ..
07/26/2026  07:26 PM    <DIR>          core
07/26/2026  07:20 PM                 0 db.sqlite3
07/26/2026  07:20 PM    <DIR>          firstProject
07/26/2026  07:07 PM               690 manage.py
               2 File(s)            690 bytes
               4 Dir(s)   2,664,497,152 bytes free

(.venv) D:\py\firstProject>



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
