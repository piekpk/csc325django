# csc325django

Django starter project for CSC325 coursework (mirrors the professor's demo layout:
project package + `csc325myapp` app + a virtual environment named `myvm`).

## Setup on your PC (Windows)

```powershell
cd C:\path\to\csc325django
python -m venv myvm
myvm\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

The dev server starts at http://127.0.0.1:8000/

## Common gotcha (from the professor's demo)

`python -m manage.py runserver` **fails** with `ModuleNotFoundError` — the `-m`
flag expects a module name, not a file. Use either of these instead:

```powershell
python manage.py runserver      # file name, no -m
python -m manage runserver      # module name, no .py
```

## What's included

- `csc325/` — Django project package (`settings.py` has `csc325myapp` registered)
- `csc325myapp/` — app scaffold (views/models are blank for you to fill in)
- `manage.py`, `requirements.txt` (pinned to Django 6.1.2)
- `db.sqlite3` is gitignored; run `migrate` after cloning
