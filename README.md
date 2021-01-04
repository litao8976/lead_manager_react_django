1. python3 --version
2. pip3 install pipenv
3. PYTHON_BIN_PATH="$(python3 -m site --user-base)/bin"
   PATH="$PATH:$PYTHON_BIN_PATH"

4. pipenv shell
5. pipenv install django djangorestframework django-rest-knox
6. django-admin startproject leadmanager  
7. python manage.py startapp leads
8. python manage.py makemigrations leads
9. python manage.py migrate

# Install Postgres
pip install psycopg2-binary
pg_ctl -D /usr/local/var/postgres start

psql postgres

create role app_user with login password 'app_password';

alter role app_user createdb;

\du

\q

psql postgres -U app_user

create database app_database;

\connect app_database;

# Lead Manager

> Full stack Django/React/Redux app that uses token based authentication with Knox.

## Quick Start

```bash
# Install dependencies
npm install

# Serve API on localhost:8000
pipenv shell
python leadmanager/manage.py runserver

# Run webpack (from root)
npm run dev

# Build for production
npm run build
```
