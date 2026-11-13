# Django Online Shop

A historical Django e-commerce catalog project built with Python, PostgreSQL, and Docker.
This repository preserves an older development snapshot and is not production-ready.

## Implemented features

- Product listing, product details, pricing, and active/inactive status.
- Product comments and ratings with admin moderation.
- Custom user model and account authentication.
- Persian localization and translation support.
- Django admin interface.
- Docker Compose setup for Django and PostgreSQL.

## Local development

The project uses historical dependencies, including Django 4.0.2 and Python 3.9.
Review its dependencies and configuration before running it on a modern system.

1. Install Docker and Docker Compose.
2. Copy `.env.example` to `.env` and set a unique `DJANGO_SECRET_KEY`.
3. Start the services:

```powershell
docker compose up --build
```

4. Apply migrations:

```powershell
docker compose exec web python manage.py migrate
```

The included PostgreSQL `trust` authentication is for isolated local development only.
No production deployment or automated test results are claimed for this snapshot.
