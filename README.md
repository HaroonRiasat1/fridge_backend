# Fridge app: backend

Django REST backend for **Fridge**, a mobile app that scans groceries to track expiry dates and suggests recipes. Built as a team project at Åbo Akademi University; it was a finalist at ICT Showroom 2025, winning Best UI from the jury plus first place for Best Technical Content and Best Presentation in the public vote.

The Flutter app is in [fridge_flutter](https://github.com/HaroonRiasat1/fridge_flutter).

## Credits

Team project. This repository is a snapshot of [zaper1402/fridge_backend](https://github.com/zaper1402/fridge_backend); the original commit history is by Ashir Kulshreshtha.

## Stack

Django and Django REST Framework, PostgreSQL on AWS RDS, Firebase Admin.

## Run locally

Create a `.env` file:

```
DJANGO_SECRET_KEY=...
DB_NAME=...
DB_USER=...
DB_PASSWORD=...
DB_HOST=...
DB_PORT=5432
```

Put the Firebase Admin service-account JSON at the path referenced in `fridge/settings.py` (it is gitignored). Then:

```bash
python -m venv venv
```

```bash
source venv/bin/activate
```

```bash
pip install -r requirements.txt
```

```bash
python manage.py migrate
```

```bash
python manage.py runserver
```
