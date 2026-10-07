# csc325django

Django starter project for CSC325 coursework.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

The dev server starts at http://127.0.0.1:8000/

## What's included

- Stock `django-admin startproject` scaffold (`csc325` project package + `manage.py`)
- `requirements.txt` pinned to Django 6.1.2
