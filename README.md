# Ex02 Django ORM Web Application
## Date: 28.04.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



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
from .models import Movie

admin.site.register(Movie)
models.py
from django.db import models

class Movie(models.Model):
    title = models.CharField(max_length=200)
    director = models.CharField(max_length=100)
    release_year = models.PositiveIntegerField()
    genre = models.CharField(max_length=100)

    def _str_(self):
        return f"{self.title} ({self.release_year})"

```
## OUTPUT
![web ex 2](https://github.com/user-attachments/assets/2888da23-00cf-4912-bb26-7406c76051e9)


     
## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
