
# Django To-Do List Application

This is a basic Django application for managing tasks. Users can add, view, and delete tasks. 
It is designed as an introduction to Django for learning its core concepts like models, views, templates, and URL routing.

## Features

- Add new tasks with a title and description.
- View a list of all tasks.
- Delete tasks.
- Manage tasks in a SQLite database.

## Requirements

- Python 3.8+
- Django 5.1+

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd todo_project
   ```

2. Create a virtual environment and activate it:
   - **Linux/Mac**:
     ```bash
     python3 -m venv env
     source env/bin/activate
     ```
   - **Windows**:
     ```bash
     python -m venv env
     env\Scripts\activate
     ```

3. Install Django:
   ```bash
   pip install django
   ```

4. Run migrations to set up the database:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. Start the development server:
   ```bash
   python manage.py runserver
   ```

6. Open the application in your browser:
   - Main application: [http://127.0.0.1:8000/](http://127.0.0.1:8000/)
   - Admin panel: [http://127.0.0.1:8000/admin/](http://127.0.0.1:8000/admin/)

## Folder Structure

```
todo_project/
│
├── tasks/
│   ├── migrations/
│   ├── templates/
│   │   └── tasks/
│   │       ├── task_list.html
│   │       └── add_task.html
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── views.py
│
├── todo_project/
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── db.sqlite3
├── manage.py
└── env/
```

## Future Improvements

- Add authentication for users to manage their own tasks.
- Implement task completion toggle.
- Enhance the UI using CSS frameworks like Bootstrap.
- Provide an API using Django REST Framework.

## Author

Created by [Your Name].
