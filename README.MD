# Online Banking System

This is a Online Banking basic app created using Django Framework.

## Features

* Create an online bank Account.
* Sign in to online bank account using Account Number & password.
* Deposit & Withdraw Money.
* Transaction Detail Page.
* Calculate Monthly Interest.

## Requirements

+ Python >= 3.6.3
+ pip install -r requirements.txt at the root of your project


## Install Redis Server

[Redis Quick Start](https://redis.io/topics/quickstart)

Run Redis server
```bash
redis-server
```

## Project Installation

To setup a local development environment:

## For Mac

```bash
virtualenv venv            # create a virtualenv
source venv/bin/activate   # activate the Python virtualenv 
```

## For Windows

```bash
virtualenv venv            # create a virtualenv
venv\scripts\activate   # activate the Python virtualenv 
```


or with [virtualenvwrapper](http://virtualenvwrapper.readthedocs.org/en/latest/),
```bash
mkvirtualenv -p python3 {{project_name}}   # create and activate environment
workon {{project_name}}   # reactivate existing environment
```

Migrate Database,
```bash
python manage.py migrate
```

Run the web application locally,
```bash
python manage.py runserver # 127.0.0.1:8000
```

Create Superuser,
```bash
python manage.py createsuperuser
```

Run Celery
(Different Terminal Window with Virtual Environment Activated)
```bash
celery -A bankingsystem worker -l info

celery -A bankingsystem beat -l info
```
