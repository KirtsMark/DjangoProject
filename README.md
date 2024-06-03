# Getting Started Guide
## This document is a guide to creating a new django project that uses:

windows__
python3.8.2__
pip__
django 2.2.15 (LTS)__
virtualenv__
Redis__
django channels 2__
Postgres__

## Install Python3.8.2
Bottom of page: https://www.python.org/downloads/release/python-382/__

## Installing pip
https://pypi.org/project/pip/__
Open cmd prompt__
pip install pip__
Setup virtualenv__

## Navigate to where you want to keep your django projects. I use D://DjangoProjects/
Create D://DjangoProjects/ChatServerPlayground folder or whatever you want to name the project.__
Create a virtual environment to run the project in.__
Typically I call it "venv" but you can call it something else if you like. Doesn't matter. djangoproject_venv for example.__
python -m venv venv or python -m venv djangoproject_venv if you like__
Open a cmd prompt in your project directly__
Navigate into venv folder__
cd venv__

## Activate the virtual environment__
Windows: Scripts\activate__
Linux: source bin/activate__
Mac (I think): source bin/activate__
Install Django and create Django project__

## Install django
python -m pip install Django==2.2.15__
See LTS: https://www.djangoproject.com/download/__


## Create the django project
django-admin startproject ChatServerPlayground__
Rename root directory (ChatServerPlayground) to src__
I prefer to name my root directory src__
So now you should have the following folder structure:__
D://DjangoProjects/ChatServerPlayground/venv/src/
Inside src you will have a folder name ChatServerPlayground and a manage.py file__
Keep track of the libraries you use__
pip freeze > requirements.txt__

### Run the server to make sure it's working
python manage.py runserver__
Visit http://127.0.0.1:8000/
