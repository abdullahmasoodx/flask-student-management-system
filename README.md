# Flask MySQL CRUD Starter

A Flask CRUD starter template using SQLAlchemy and MySQL.

---

## Overview

A simple but complete CRUD web application built with Flask, SQLAlchemy, and MySQL.
Good starting point if you want to learn how Flask connects to a real database.

- Backend logic using Flask
- Database integration using SQLAlchemy
- Clean UI using Bootstrap

---

## Features

- Add new students
- View all students
- Edit student details
- Delete student
- Flash messages (success, update, delete alerts)
- Responsive Bootstrap UI

---

## Tech Stack

- **Backend:** Flask
- **Database:** MySQL
- **ORM:** SQLAlchemy
- **Driver:** PyMySQL
- **Frontend:** HTML, Bootstrap 5

---

## Project Structure
```
flask-mysql-crud-starter/
│
├── app.py
├── config.py
├── models.py
├── requirements.txt
│
├── templates/
│   ├── base.html
│   ├── index.html
│   ├── add_student.html
│   └── edit_student.html
│
├── static/
└── screenshots/
```

---

## Screenshots

### Home Page
![Home](screenshots/home.png)

### Add Student
![Add](screenshots/add.png)

### Success Message
![Success](screenshots/success.png)

---

## Setup

### 1. Clone the repository
```bash
git clone https://github.com/your-username/flask-mysql-crud-starter.git
cd flask-mysql-crud-starter
```

### 2. Create a virtual environment
```bash
python -m venv venv
```

Activate it:

**Windows:**
```bash
venv\Scripts\activate
```

**Mac/Linux:**
```bash
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Create the MySQL database
```sql
CREATE DATABASE flask_crud_db;
```

### 5. Configure the database

Update `config.py` with your credentials:
```python
SQLALCHEMY_DATABASE_URI = "mysql+pymysql://root:password@localhost/flask_crud_db"
SECRET_KEY = "your_secret_key"
```

### 6. Run the app
```bash
python app.py
```

### 7. Open in your browser
```
http://127.0.0.1:5000
```

---

## Security Notes

- Never hardcode your `SECRET_KEY` in production
- Use environment variables for credentials
- Don't commit `.env` files or passwords to Git
- Generate a strong key with `python -c "import secrets; print(secrets.token_hex(32))"`

---

## Planned Features

- User authentication (login/register)
- Search and filtering
- Pagination
- REST API version
- Docker support
- Deployment guide (Render / AWS / VPS)

---

## Contributing

Pull requests are welcome. Open an issue first if you're planning something bigger.
