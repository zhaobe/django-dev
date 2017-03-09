# django-dev

## Setting up Django:
- if you want to use Django with a database, make sure to setup either PostgreSQL, MySQL, Oracle or SQLite.
- install `pip` if you have not.
- use `python -c "import django; print(django.__path__)"` to find if you have Django already installed.

- setup virtualenv, refer to [this](https://virtualenv.pypa.io/en/stable/installation/)

## Using virtualenv
- once you install virtualenv, you may `cd` to your target directory and make a virtual environment with `virtualenv env`.
- make sure you are in the root directory, type `source ./env/bin/activate` and you should see `(env)` in your command line.
- to deactivate the virtualenv, use `deactivate`, unless error says otherwise.

- activate virtualenv, and use `pip install django`, to install Django, refer to [this](https://docs.djangoproject.com/en/1.10/topics/install/#installing-official-release)
- use `which django-admin.py` to confirm your newly installed Django within your virtual environment.

- there is a gitignore for python so env or venv dependencies won't conflict with collaboration.

## Setup Project
- good reference from [mozilla] (https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/development_environment)
- same reference from [django] (https://docs.djangoproject.com/en/1.10/intro/tutorial01/)

## Part 2 - Database Checklist
- `python manage.py makemigrations`, makemigrations tells Django there were changes to the models and you would like to store them as migration. Run this command to create migrations for those changes.
- `python manage.py migrate`, to apply changes to the database.
- `python manage.py check`, checks for any problems in the project without touching the database.
- Playing with API section is familiarized, may refer back if confused.
- Added super user and once server is activated `python manage.py runserver`, go to `http://127.0.0.1:8000/admin/` for login.

## Handy Commands
- `python manage.py runserver` will run the server
- `python manage.py shell` will run the shell 
- `python manage.py test polls` will look for tests in polls application and run a mock db for testing

## Advanced tutorial: Writing reusable apps
### Setup
- make sure you have the virtual env running
- then we will install setuptools with `pip install setuptools`
- you might get a couple messages saying `Requirement already satisfied: ...`
- next you will need to `pip install distribute` also
