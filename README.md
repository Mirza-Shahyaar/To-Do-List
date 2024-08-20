# To-Do List Application with User Login

This is a full-stack To-Do List web application built with Django. The application allows users to create, update, and delete tasks. It includes user authentication, so each user can manage their own to-do list after logging in.

## Features

- **User Registration & Login**: Users can register, log in, and log out. Each user has their own to-do list.
- **Task Management**: Users can add, update, delete, and mark tasks as completed.
- **Responsive Design**: The app is designed to be responsive and works well on both desktop and mobile devices.
- **Database Integration**: Task data and user information are stored in a relational database (SQLite by default).
- **Secure Password Storage**: User passwords are securely hashed using Django’s built-in authentication system.

## Prerequisites

Before running the project, ensure you have the following installed:

- **Python 3.x**
- **Django**
- **pip** (Python package manager)
- **Virtualenv** (optional but recommended)

You can install Django and other dependencies using pip:

```bash
pip install django
```

## Project Setup

### 1. Clone the Repository

Clone the project repository to your local machine:

```bash
git clone https://github.com/your-username/todo-list-django.git
cd todo-list-django
```

### 2. Create a Virtual Environment (Optional but recommended)

Create and activate a virtual environment to isolate the project dependencies:

```bash
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```

### 3. Install Dependencies

Install the required Python packages:

```bash
pip install -r requirements.txt
```

### 4. Apply Migrations

Apply the database migrations to set up the database schema:

```bash
python manage.py migrate
```

### 5. Create a Superuser

Create a superuser account to access the Django admin interface:

```bash
python manage.py createsuperuser
```

### 6. Run the Development Server

Start the Django development server:

```bash
python manage.py runserver
```

Visit `http://127.0.0.1:8000/` in your web browser to view the application.

## Project Structure

- `todo/`: The main Django project directory.
- `tasks/`: The Django app responsible for handling tasks.
- `users/`: The Django app responsible for user authentication and profile management.
- `templates/`: HTML templates for rendering the web pages.
- `static/`: Static files like CSS, JavaScript, and images.
- `db.sqlite3`: The SQLite database file (created after running migrations).

## Usage

### User Registration and Login

1. **Register**: Navigate to the registration page and create a new account.
2. **Login**: After registration, log in with your credentials.
3. **Logout**: You can log out from the account at any time.

### Managing Tasks

1. **Add Task**: After logging in, you can add a new task to your to-do list.
2. **Update Task**: Edit an existing task to change its details.
3. **Delete Task**: Remove a task from your to-do list.
4. **Mark as Completed**: Check off tasks when they are done.

## Customization

You can customize the application by modifying the templates, views, and models according to your needs. The project is set up to be easily extendable.

### Adding More Features

- **Priority Levels**: Add priority levels to tasks (e.g., High, Medium, Low).
- **Due Dates**: Allow users to set due dates for tasks.
- **Notifications**: Implement email or in-app notifications for task deadlines.

## Deployment

To deploy the project to a production environment, you will need to:

1. **Configure the Database**: Switch to a production-grade database like PostgreSQL or MySQL.
2. **Set Up Static Files**: Configure static file serving with tools like `whitenoise` or a cloud storage service.
3. **Deploy with WSGI/ASGI**: Use a WSGI server like Gunicorn and a reverse proxy like Nginx.
4. **Secure the Application**: Ensure the application is secured with HTTPS and proper environment variables for sensitive settings.

## Acknowledgements

- Django Documentation: [Django Project](https://www.djangoproject.com/)
- Bootstrap for CSS: [Bootstrap](https://getbootstrap.com/)

---
