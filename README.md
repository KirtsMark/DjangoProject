# Getting Started Guide
## This document is a guide to creating a new django project that uses:

windows
python3.8.2
pip
django 2.2.15 (LTS)
virtualenv
Redis
django channels 2
Postgres

## Install Python3.8.2
Bottom of page: https://www.python.org/downloads/release/python-382/

## Installing pip
https://pypi.org/project/pip/
Open cmd prompt
pip install pip
Setup virtualenv

## Navigate to where you want to keep your django projects. I use D://DjangoProjects/
Create D://DjangoProjects/ChatServerPlayground folder or whatever you want to name the project.
Create a virtual environment to run the project in.
Typically I call it "venv" but you can call it something else if you like. Doesn't matter. djangoproject_venv for example.
python -m venv venv or python -m venv djangoproject_venv if you like
Open a cmd prompt in your project directly
Navigate into venv folder
cd venv

## Activate the virtual environment
Windows: Scripts\activate
Linux: source bin/activate
Mac (I think): source bin/activate
Install Django and create Django project

## Install django
python -m pip install Django==2.2.15
See LTS: https://www.djangoproject.com/download/


## Create the django project
django-admin startproject ChatServerPlayground
Rename root directory (ChatServerPlayground) to src
I prefer to name my root directory src because inside the project is another folder named ChatServerPlayground or whatever you called your project
So now you should have the following folder structure:
D://DjangoProjects/ChatServerPlayground/venv/src/
Inside src you will have a folder name ChatServerPlayground and a manage.py file
Keep track of the libraries you use
pip freeze > requirements.txt

### Run the server to make sure it's working
python manage.py runserver
Visit http://127.0.0.1:8000/
