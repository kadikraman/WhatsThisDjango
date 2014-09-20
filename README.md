WhatsThisDjango
===============

**TL;DR:** I'm learning Django. Let's trial and error some of this stuff!

## Installation instructions to get Django running: [(Here they are!)](https://docs.djangoproject.com/en/1.7/topics/install/)
1. Install [Python](https://www.python.org/download). I'm going with Python 3.
2. Install [pip](https://pip.pypa.io/en/latest/installing.html#install-pip). This is the package manager for Python. For the Windows lot, you'll probably need to add the Scripts folder in your Python directory to your path manually.
3. For non-windows: "sudo pip install Django". For Windows, open the command prompt as an administator and run "pip install Django". This will install Django in your Python installation’s site-packages directory.

## Setup dev environment
1. Nagivate in the solution to where manage.py lives and run "run python manage.py migrate" - this will sync all the changes in the database and in the models.
2. And finally to run the app: in the same directory as above run "python manage.py runserver 8080" which will start the webserver at http://localhost:8080/

Here's the tutorial I'm following. [(Link)](https://docs.djangoproject.com/en/1.7/intro/tutorial01/)

Remember there's a 3 step guide to making model changes:
1. Change your models (in models.py).
2. Run python manage.py makemigrations to create migrations for those changes
3. Run python manage.py migrate to apply those changes to the database.