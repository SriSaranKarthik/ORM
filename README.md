# Ex02 Django ORM Web Application
## Date: 06/10/2025

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![](<car er diagram.jpg>)

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
## 1.ADMIN.PY
```PYTHON
from django.contrib import admin
from .models import Car

admin.site.register(Car)
class CarAdmin(admin.ModelAdmin):
    list_display = ('id', 'brand', 'model', 'year', 'price')
```
## 2.MODELS.PY
```PYTHON
from unittest.util import _MAX_LENGTH
from django.db import models

from django.forms import IntegerField
# Create your models here.

class Car(models.Model):
    id = models. IntegerField(primary_key=True)
    brand = models.CharField(max_length=15)
    model = models. CharField(max_length=30)
    year = models. DateField()
    price = models. IntegerField()
    type = models.CharField(max_length=10)
```


## OUTPUT

![](<Screenshot 2025-10-06 092553.png>)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
