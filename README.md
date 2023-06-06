# Django ORM Web Application
# AIM

To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

Include your ER diagram here
![image](https://github.com/niveshaprabu/django-orm-app/assets/122986499/1e8019bd-6839-4523-bb60-924d5db169d2)


# DESIGN STEPS
# STEP 1:

  clone the repository from github.
# STEP 2:

  create an admin interface for Django.
# STEP 3:

  create an app and edit settings.py.
# STEP 4:

  Makemigratons and migrate the changes.
# PROGRAM

'''

admin.py

from django.contrib import admin

from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)

models.py

from django.db import models

from django.contrib import admin

class Student (models.Model):

referencenumber=models.CharField(max_length=20,help_text="reference number")

name=models.CharField(max_length=100)

age=models.IntegerField()

email=models.EmailField()

class StudentAdmin(admin.ModelAdmin):

list_display=('referencenumber','name','age','email')

'''
# OUTPUT
![WhatsApp Image 2023-06-06 at 22 31 33](https://github.com/niveshaprabu/django-orm-app/assets/122986499/92ea6da0-2a83-46a0-a9b6-cc6347ca1592)


# RESULT
The program for creating an student database using ORM is executed successfully.
