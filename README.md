# University Management System Django

University Management System Django is a complete campus management platform built with Django.
It supports administration, staff, students, courses, sessions, semesters, quizzes, results, and payments.

## Owner

- Project owner: HafizullahKhokhar1
- Copyright: HafizullahKhokhar1
- Repository: https://github.com/HafizullahKhokhar1/University-Management-System-Django

## Features

- Admin dashboard with academic and user management
- Student and lecturer management workflows
- Program and course allocation
- Session and semester controls
- Quiz and assessment modules
- Grade and result generation
- Payment and invoice support
- Multi-language support

## Tech Stack

- Python
- Django
- SQLite (default)
- Bootstrap 5

## Quick Start

1. Clone the repository.
2. Create a virtual environment.
3. Install requirements.
4. Run migrations.
5. Start the development server.

```powershell
python -m venv venv
.\venv\Scripts\Activate.ps1
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

Open http://127.0.0.1:8000/

## Test Credentials

Use the test credentials you created in your local environment.

## Project Structure

- accounts: user roles, profile logic, auth utilities
- core: dashboard, news/events, sessions and semesters
- course: programs, courses, registration and allocation
- quiz: quiz engine and progress tracking
- result: score management and grade processing
- payments: invoice and payment workflows
- templates/static: UI templates and assets

## Deployment Notes

- Set environment variables in `.env`
- Configure `ALLOWED_HOSTS` for production
- Use a production database and secure secret key

## License

This project is proprietary and all rights are reserved by HafizullahKhokhar1.
See LICENSE for details.
