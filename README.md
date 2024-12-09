
# Django Todo List Application

A simple Django-based Todo List application where you can add, view tasks efficiently. 

---

## **Features**
- Add tasks with titles, descriptions, and a completion status.
- View a list of tasks in a clean and simple UI.
- Track creation timestamps for each task.
- PostgreSQL database integration for data persistence.

---

## **Technologies Used**
- **Backend:** Django (Python)
- **Frontend:** HTML, CSS
- **Database:** PostgreSQL
- **Environment Management:** Virtual Environment (venv)

---

## **Getting Started**

### **Prerequisites**
Ensure you have the following installed:
- Python (3.8 or newer)
- PostgreSQL
- pip (Python package installer)

---

### **Project Setup**

#### **1. Clone the Repository**
```bash
git clone https://github.com/PRANAVK3004/Todo_django.git
cd Todo_django
```

#### **2. Set Up a Virtual Environment**
```bash
python3 -m venv env
source env/bin/activate  # On Windows, use `env\Scripts\activate`
```

#### **3. Install Dependencies**
 Manually install Django:
```bash
pip install django
```

---
## **START AND ADD Migrations **
# Create Django project
django-admin startproject todo_project
cd todo_project

# Create Django app
python manage.py startapp tasks

# Run migrations
python manage.py makemigrations
if todo_tasks is not there in migrations:
python manage.py makemigrations todo_tasks

python manage.py migrate

# Run server
python manage.py runserver


### **Database Configuration**

1. Open the `settings.py` file in the `todo_project` directory.
2. Update the `DATABASES` configuration to match your PostgreSQL setup:
   ```python
   DATABASES = {
       'default': {
           'ENGINE': 'django.db.backends.postgresql',
           'NAME': 'todo_db',          # Replace with your database name
           'USER': 'postgres',         # Replace with your PostgreSQL username
           'PASSWORD': ' ',    # Replace with your PostgreSQL password
           'HOST': 'localhost',        # Replace if using a remote database
           'PORT': '5432',             # Default PostgreSQL port
       }
   }
   ```

3. Create the PostgreSQL database if not already created:
   ```sql
   CREATE DATABASE todo_db;
   ```

---

### **Database Migrations**
Run the following commands to set up your database:
```bash
python manage.py makemigrations
python manage.py migrate
```

---

### **Run the Development Server**
Start the server to test the application:
```bash
python manage.py runserver
```
Open your browser and navigate to `http://127.0.0.1:8000/`.

---

### **Admin Panel of PostgreSQL(Optional)**
If you need access to Django's admin panel:
1. Create a superuser:
   ```bash
   python manage.py createsuperuser
   ```
2. Access the admin panel at `http://127.0.0.1:8000/admin/`.

---





## **Future Enhancements**
- Add user authentication to allow personalized task management.
- Implement task categorization and due dates.
- Add an API layer for third-party integrations.

---




## **Contact**
For any  issues, reach out via the repository's (https://github.com/PRANAVK3004/Todo_django/issues).
or you can contact to kumbhojkarpranav2@gmail.com
