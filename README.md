# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

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
models.py
from django.db import models

class Car(models.Model):
    brand = models.CharField(max_length=100)
    model_name = models.CharField(max_length=100)
    year = models.IntegerField()
    price = models.DecimalField(max_digits=10, decimal_places=2)
    available = models.BooleanField(default=True)

    def __str__(self):
        return f"{self.brand} {self.model_name} ({self.year})"
    
admin.py
from django.contrib import admin
from .models import Car

admin.site.register(Car)

## OUTPUT

Include the screenshot of your admin page.

![alt text](<WhatsApp Image 2025-09-13 at 11.19.09_696da67e.jpg>)

![alt text](<Screenshot 2025-09-15 090246.png>)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
