# Online Shop with Oscar-Django

## Create entorno virtual
virtualenv entorno_virtual -p python3

## Active entorno virtual
source entorno_virtual/bin/activate

## install Oscar and dependencies for postgres DB
$ pip install django-oscar[sorl-thumbnail]
$ django-admin startproject onlineshop
$ pip install psycopg2
$ pip install pysolr

## Documentation
https://django-oscar.readthedocs.io/en/3.2a/internals/getting_started.html

## create base de datos (postgres)
CREATE DATABASE dbonlineshop WITH OWNER test;
$ python manage.py migrate

## populate countries
$ pip install pycountry
$ python manage.py oscar_populate_countries

## run app
$ python manage.py runserver

## create an superuser
$ python manage.py createsuperuser
javier
2525_ap
email@gmail.com
