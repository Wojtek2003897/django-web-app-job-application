# Job Application Django App

A simple web application built with Django that allows users to submit a job application form. The app stores submitted data in a database and sends a confirmation email to the applicant.

---

## Features

* Submit job applications via a clean web form
* Store applicant data in a database (SQLite)
* Send email confirmation after submission
* Display success messages to users
* Navigation bar with multiple pages (Home & About)

---

## How It Works

1. User fills out a job application form (first name, last name, email, date, occupation)
2. Form is submitted via POST request
3. Data is validated and saved to the database
4. A confirmation email is sent to the user
5. A success message is displayed on the page

---

## 🛠️ Tech Stack

* Python
* Django
* SQLite
* Bootstrap 5
* HTML (Django Templates)

---

## Model

**Form**

* first_name
* last_name
* email
* date
* occupation

---

## Running the Application

Start the development server:

```bash
python manage.py runserver
```

Open in browser:

```
http://127.0.0.1:8000/
```

---

## Email Configuration

The app sends emails using Gmail SMTP.

Update `settings.py`:

```python
EMAIL_BACKEND = 'django.core.mail.backends.smtp.EmailBackend'
EMAIL_HOST = 'smtp.gmail.com'
EMAIL_PORT = 587
EMAIL_USE_TLS = True
EMAIL_HOST_USER = '<your-email>'
EMAIL_HOST_PASSWORD = '<your-app-password>'
```

Important:

* Use Gmail **App Password**, not your real password

---

## Routes

* `/` → Job application form
* `/about/` → About page





