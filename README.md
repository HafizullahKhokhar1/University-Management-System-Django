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

## Easy Deployment (Testing)

You can deploy this project quickly for testing on Render or Railway.

### Option 1: Render (Fastest)

1. Push code to GitHub (already done).
2. In Render, create a new Web Service from this repository.
3. Render will detect `render.yaml` automatically.
4. Deploy and open the generated URL.

### Option 2: Railway

1. Create a new Railway project from your GitHub repository.
2. Set start command to: `gunicorn config.wsgi:application`
3. Set build command to: `pip install -r requirements.txt && python manage.py migrate && python manage.py collectstatic --noinput`
4. Add env vars: `DEBUG=False`, `SECRET_KEY`, `ALLOWED_HOSTS`, `CSRF_TRUSTED_ORIGINS`.

### Notes

- `Procfile` and `runtime.txt` are included for platform compatibility.
- Current default DB is SQLite, fine for testing but not recommended for production.

## License

This project is proprietary and all rights are reserved by HafizullahKhokhar1.
See LICENSE for details.

## Contributing

Contributions are welcome under the contribution policy in CONTRIBUTING.md.
By contributing, you agree that accepted contributions are assigned to HafizullahKhokhar1.
