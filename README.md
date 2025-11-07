<h1 align="center" style="color:#b026ff;">⚡ Django REST API — Login Authentication</h1>

<p align="center" style="color:#b8b8ff;">
 A minimal DRF project implementing JWT-based login authentication.<br>

</p>

---

##  Overview
This project is a **Django REST Framework (DRF)** implementation focused purely on authentication.  
It provides one endpoint:

```bash
POST /api/login/
```
Accepts `username` and `password`, returns a **JWT token** on successful authentication.



## ⚙️ Features
- ✅ Simple JWT login via `/api/login/`
- 🔐 Accepts `username` & `password`
- 🧾 Returns **JWT access token**
- 👤 Includes test user credentials for quick testing



## 💻 Installation

```bash
# Create Django project and app
django-admin startproject myproject_name
cd myproject
python manage.py startapp api

# Create and activate a virtual environment (optional)
python -m venv venv
source venv/bin/activate     # On Windows: venv\Scripts\activate

# Install dependencies
pip install django djangorestframework djangorestframework-simplejwt

```

Test User Credentials:
Username: testuser
Password: testpass123
```bash

#Run the Django Server 
python manage.py runserver
```
Endpoint:
POST /api/login/
```bash

Request Body:
{
  "username": "testuser",
  "password": "testpass123"
}


Response:
{
  "access": "<Generated_access_token>"
}
```


