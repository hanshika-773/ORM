# Ex02 Django ORM Web Application
## Date: 21.03.24

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).
### Entity Relationship Diagram
![Screenshot 2024-03-22 131648](https://github.com/hanshika-773/ORM/assets/153576501/2a582bae-3d1d-4712-8b98-ce8755c3ab40)

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
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

models.py
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')
```
## OUTPUT

![alt text](<Screenshot 2024-03-21 144926.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
