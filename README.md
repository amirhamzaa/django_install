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
