# Ex02 Django ORM Web Application
## Name: K DHANUSRI POOJA
## Register Number: 212224040068
## Date: 11.04.2025


## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

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
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)

models.py

from django.db import models
from django.contrib import admin
class Movie(models.Model):
    mid=models.IntegerField()
    mname=models.CharField(max_length=100)
    collection=models.IntegerField()
    year=models.IntegerField()
    rating=models.FloatField()

class MovieAdmin(admin.ModelAdmin):
    list_display=('mid','mname','collection','year','rating')

```

## OUTPUT

![Screenshot 2025-04-11 133316](https://github.com/user-attachments/assets/19fe0b7e-e837-491d-ada7-9dfd1ffa1869)



## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
