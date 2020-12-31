1. python3 --version
2. pip3 install pipenv
3. PYTHON_BIN_PATH="$(python3 -m site --user-base)/bin"
   PATH="$PATH:$PYTHON_BIN_PATH"

4. pipenv shell
5. pipenv install django djangorestframework django-rest-knox
# Lead Manager

> Full stack Django/React/Redux app that uses token based authentication with Knox.

## Quick Start

```bash
# Install dependencies
npm install

# Serve API on localhost:8000
python leadmanager/manage.py runserver

# Run webpack (from root)
npm run dev

# Build for production
npm run build
```
