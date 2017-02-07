# django-dev

## Setting up Django:
- if you want to use Django with a database, make sure to setup either PostgreSQL, MySQL, Oracle or SQLite.
- install `pip` if you have not.

- setup virtualenv, refer to [this](https://virtualenv.pypa.io/en/stable/installation/)
- install Django with `pip install Django`, refer to [this](https://docs.djangoproject.com/en/1.10/topics/install/#installing-official-release)

## Using virtualenv
- once you install virtualenv, you may `cd` to your home directory and make a directory to hold your virtual environment.
- `cd` into the new directory and use `python -m venv <nameOfVirtualEnv>`, replace nameOfVirtualEnv with your choice. You may use python or python3 to create the venv, either is fine.
- then use `virtualenv venv --distribute`, you should see a new python executable being created and installing of other tools.
- to activate the virtualenv, use `source venv/bin/activate`.
- to deactivate the virtualenv, use `deactivate`, unless error says otherwise.
