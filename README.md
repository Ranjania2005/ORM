# Ex02 Django ORM Web Application
## Date: 01/03/2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![alt text](<WhatsApp Image 2024-03-01 at 20.50.38_8ae4a590.jpg>)

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
from .models import Book,BookAdmin
admin.site.register(Book,BookAdmin)

models.py
from django.db import models
from django.contrib import admin
class Book(models.Model):
   bookid=models.IntegerField(primary_key=True);
   bookname=models.CharField(max_length=30);
   authorname=models.CharField(max_length=20);
   bookprize=models.IntegerField();
   contemail=models.EmailField();
class BookAdmin(admin.ModelAdmin):
   list_display=("bookid","bookname","authorname","bookprize","contemail");
```

## OUTPUT

![alt text](<Screenshot (130).png>)

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
