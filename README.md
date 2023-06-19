

# Project's Title
**TechnicalDebtApp**, I named the project TechnicalDebtApp because I wanted to do something for my work and is also my exam app to get the certification from the Coding Factory 3 (educational program in software development) of the Athens University of Economics and Business https://codingfactory.aueb.gr/ so I combine them.

## Project Description
I made this app to store all the orders and repairs we do in the technical department where I work. Users will have separate licenses depending on the type of work they do, now every repair and order will be user named so I know who did it (which is complicated now) and can communicate with them. It's an early version that I hope to develop even more in the future and add more actions and tools (like searching in lists).

## Technologies used
Python 3.11.3
Django 4.2.2
djangorestframework 3.14.0 (API)
drf-spectacular 0.26.2 (documentation)
Bootstrap 5.2 (front-end)


## INSTALLATION:
Download the app, open a terminal at the main folder of the project.

Create a virtual environment (need Python to be installed):
python -m venv .venv

Activate the environment:
```
.venv\scripts\activate
```

Install the requirements:
```
pip install -r requirements.txt
```

Run the server:
```
python manage.py runserver 
```

Open a browser and go to:
http://127.0.0.1:8000/


The project already have users and data:
username: admin password: 1234
username: user1 password: 123qwe!@# (Note: he have some restrictions at supplier views)
username: user2 password: 123qwe!@#
username: user3 password: 123qwe!@# (Note: he have some restrictions at supplier views)


### Run on local network
Change at settings.py the bellow:
DEBUG = False
ALLOWED_HOSTS = ['*']

Then run server with:
```
python manage.py runserver pc-ip:8000 e.x: python manage.py runserver 192.168.1.2:8000
```
or
```
python manage.py runserver 0.0.0.0:8000
```

## Test's
Activate the environment:
```
.venv\scripts\activate
```

Run the test:
```
python manage.py test
```

At the app I have some model tests and login urls tests (API and front-end).
The other views have a login_required decorator and the simple test's can't run (need to login inside the test)

## Future updates:
Search views
Better templates (some can be merged and/or used from more views)
Complete users managment form front-end


list   ordering = ['-updated_at']
