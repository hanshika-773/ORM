# Ex02 Django ORM Web Application
## Date: 11.03.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![2](https://github.com/hanshika-773/ORM/assets/153576501/7712be19-e31b-4677-b429-192acb514f58)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM
```
admin.py
from django.contrib import admin
from .models import student,studentAdmin
admin.site.register(student,studentAdmin)

models.py
from django.db import models
from django.contrib import admin
class student (models.Model):
    name=models.CharField(max_length=20,help_text="student")
    rollno=models.IntegerField()
    refno=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
class studentAdmin(admin.ModelAdmin):
    list_display=('name','rollno','refno','age','email')
```
## OUTPUT

![1](https://github.com/hanshika-773/ORM/assets/153576501/c0de65b4-93dd-4984-80ca-a77bc7c20798)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
