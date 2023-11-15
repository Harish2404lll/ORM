# Ex02 Django ORM Web Application
## Date: 28.10.2023

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram


![image](https://github.com/Harish2404lll/ORM/assets/141472096/a71c85db-47bb-463c-8bf6-cfaaf492220a)


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM
```
File: Models.py

from django.db import models
from django.contrib import admin

class footballplayer (models.Model):
    numofmatch=models.IntegerField()
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    height=models.IntegerField()

class footballplayerAdmin(admin.ModelAdmin):
    list_display=('numofmatch','name','salary','age','height')


File: Admin.py

from django.contrib import admin
from .models import footballplayer,footballplayerAdmin
admin.site.register(footballplayer,footballplayerAdmin)
```

## OUTPUT

![image](https://github.com/Harish2404lll/ORM/assets/141472096/afb699ff-10cd-458f-8152-7360ae82c477)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
