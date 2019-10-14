# rp-portfolio
A Django portfolio and blog site

## Notes

`$ mkdir personal_portfolio`

`$ cd personal_portfolio`

create virtual environment

`$ python3 -m venv venv`

activate

`$ source venv/bin/activate`

install Django

`$ pip install Django`

Create project

`$ django-admin startproject personal_portfolio`

Resulting Structure

```
rp-portfolio/
│
├── personal_portfolio/
│   ├── personal_portfolio/
│   │   ├── __init__.py
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── wsgi.py
│   │
│   └── manage.py
│
└── venv/
```

Restructure project

```
$ mv personal_portfolio/manage.py ./
$ mv personal_portfolio/personal_portfolio/* personal_portfolio
$ rm -r personal_portfolio/personal_portfolio/
```

New Structure

```
rp-portfolio/
│
├── personal_portfolio/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── venv/
│
└── manage.py
```

Startup Server

`$ python manage.py runserver`

Create app

`$ python manage.py startapp projects`


Create migration

`$ python manage.py makemigrations projects`

Create database

`$ python manage.py migrate projects`

Access Django shell

```
$ python manage.py shell
>>>
```

Import projects

`>>> from projects.models import Project`


### Admin Interface

Add to superuser

`$ python manage.py createsuperuser`
