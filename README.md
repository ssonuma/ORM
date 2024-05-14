# Ex02 Django ORM Web Application
## Date: 
14-05-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

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

## MODELS.PY:
```
from django.db import models from django.contrib import admin class Employee (models.Model): eid=models.CharField(max_length=20,help_text="Employee ID") name=models.CharField(max_length=100) salary=models.IntegerField() age=models.IntegerField() email=models.EmailField()

class EmployeeAdmin(admin.ModelAdmin): list_display=('eid','name','salary','age','email')
```
## ADMIN.PY:
```
from django.contrib import admin from .models import Employee,EmployeeAdmin

admin.site.register(Employee,EmployeeAdmin)
```


## OUTPUT
![image](https://github.com/ssonuma/ORM/assets/150653312/5d122a18-99d9-44dd-82aa-3eea4250dacc)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
