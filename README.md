# Django 2.0 Tutorial

https://docs.djangoproject.com/ja/2.0/intro/tutorial01/

## commands

```bash
python -m django --version
django-admin startproject mysite
python manage.py runserver
python manage.py runserver 8080
python manage.py startapp polls
python manage.py migrate
python manage.py makemigrations polls
python manage.py sqlmigrate polls 0001
python manage.py shell
python manage.py createsuperuser
python manage.py test polls
python -c "import django; print(django.__path__)"
```

## imports

```python
from django.http import Http404, HttpResponseRedirect, HttpResponse
from django.urls import include, path, reverse
from django.contrib import admin
from django.db import models
from django.utils import timezone
from polls.models import Question, Choice
from .models import Question
from django.template import loader
from django.shortcuts import get_object_or_404, render
from django.views import generic
from django.test import TestCase, Client
from django.test.utils import setup_test_environment
```
