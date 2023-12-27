# Flask Blog Web App

A Full Stack Blog Website with CRUD functionality 

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Installation](#installation)
- [Folder Structure](#folder-structure)
- [Technologies Used](#technologies-used)

## Overview
This project demonstrates basic CRUD functionality like Creation of posts, Updation of Posts, Deletion of Posts. Users can register, login, and manage their account.

## Features
- Account Registration and Login handled by flask_login Login Manager.
- Used Flask_Bcrypt extension for password hashing.
- Used SQLAlchemy Object-Relational Mapper(ORM) to further enhance SQL's capabilities.
- Implemented a password reset by email authentication feature through Tokens using flask_mail extension.
- Used Flask Blueprints to modularise the code, allowing for easy future extension of the project.
- Made use of packages to avoid circular imports
- Used the Python's Pillow library to handle profile pictures and fixed sizes of profile pictures, saving resources.
- Handled Forms using FlaskForm 

## Getting Started
### Installation
Clone the repository on your local machine and cd to the project folder
Setup your virtual environment by creating the following variables in the terminal
```
export FLASK_APP=run.py
```
Setup the following variables in the .bash_profile in the home directory
```
export SECRET_KEY='<A Secret Key of your choice>'
export SQLALCHEMY_DATABASE_URI='sqlite:///site.db'
export EMAIL_USER='<Your email>'
export EMAIL_PASS='<Your email password>'
```
install the following extensions and libraries using the following commands:
```
pip install flask
pip install flask_sqlalchemy
pip install flask_bcrypt
pip install flask_login
pip install flask_mail
pip install PIL
pip install flask_wtf
```
You also need to have Python3 installed on your local machine. 

```bash
# Example installation steps
git clone https://github.com/your-username/your-project.git
cd your-project
pip install -r requirements.txt
python3 app.py
```
## Folder Structure
```
.
├── README.md
├── __pycache__
│   └── run.cpython-310.pyc
├── flaskblog
│   ├── __init__.py
│   ├── __pycache__
│   │   ├── __init__.cpython-310.pyc
│   │   ├── config.cpython-310.pyc
│   │   └── models.cpython-310.pyc
│   ├── config.py
│   ├── errors
│   │   ├── __init__.py
│   │   ├── __pycache__
│   │   │   ├── __init__.cpython-310.pyc
│   │   │   └── handlers.cpython-310.pyc
│   │   └── handlers.py
│   ├── main
│   │   ├── __init__.py
│   │   ├── __pycache__
│   │   │   ├── __init__.cpython-310.pyc
│   │   │   └── routes.cpython-310.pyc
│   │   └── routes.py
│   ├── models.py
│   ├── posts
│   │   ├── __init__.py
│   │   ├── __pycache__
│   │   │   ├── __init__.cpython-310.pyc
│   │   │   ├── forms.cpython-310.pyc
│   │   │   └── routes.cpython-310.pyc
│   │   ├── forms.py
│   │   └── routes.py
│   ├── static
│   │   ├── main.css
│   │   └── profile_pics
│   │       ├── c56f8368ca1be145.jpg
│   │       └── default.jpg
│   ├── templates
│   │   ├── about.html
│   │   ├── account.html
│   │   ├── create_post.html
│   │   ├── errors
│   │   │   ├── 403.html
│   │   │   ├── 404.html
│   │   │   └── 500.html
│   │   ├── home.html
│   │   ├── layout.html
│   │   ├── login.html
│   │   ├── post.html
│   │   ├── register.html
│   │   ├── reset_request.html
│   │   ├── reset_token.html
│   │   └── user_posts.html
│   └── users
│       ├── __init__.py
│       ├── __pycache__
│       │   ├── __init__.cpython-310.pyc
│       │   ├── forms.cpython-310.pyc
│       │   ├── routes.cpython-310.pyc
│       │   └── utils.cpython-310.pyc
│       ├── forms.py
│       ├── routes.py
│       └── utils.py
├── instance
│   └── site.db
└── run.py
```


## Technologies Used
Frontend - HTML, CSS, Bootstrap
Backend - Python Flask, SQLAlchemy
Database - SQLite3
