# Django tutorial layout for HTML files 

This a simple tutorial for django with two HTML files and one layout.

## Prerequisites

`py` command should point to python3

```shell
py -V
# 3.10.0
```

## Install Git

```
git ---v or git -version
```

## Create a new folder

```shell
mkdir football stats && football stats
```
# Add .gitignore and start git

Add the following .gitignore

```shell
.venv
*.sqlite3
__pycache__
```

## Add your file to your git 

```shell
git init
git add . && git commit -m "first commit"
```

## Create virtual environment for Python and activate it

```shell
py -m venv .venv
source .venv/bin/activate
```

## Install django 

```shell
py -m pip install django
```

## Build django skeleton

Below, "core" means the core of our app, "." means build skeleton inside the current folder :

```shell
django-admin startproject core .
git add . && git commit -m "django first files"
```

## Change settings.py

Inside settings.py, add localhost to the list of allowed hosts, like this :

```
ALLOWED_HOSTS = ['localhost', '127.0.0.1']
```

## Django comes with default tables (to manage users and authorizations notably), so let's inject them into our new db :

```
py manage.py makemigrations 
py manage.py migrate 
```

## git commit

```
git add . && git commit -m "django first files"
```

## Run local server ##
```
py manage.py runserver
```
Now open your browser at localhost:8000
