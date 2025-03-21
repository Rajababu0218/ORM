# Ex02 Django ORM Web Application
# Date:19/03/2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2025-03-21 233134](https://github.com/user-attachments/assets/8c811cd8-cfb4-4070-a2ca-66f271b42d7e)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
1.models.py
```
from django.db import models
from django.contrib import admin

class Book(models.Model):
    book_no = models.CharField(max_length=100, primary_key=True)
    book_name = models.CharField(max_length=100)
    name = models.CharField(max_length=100)
    mobile_no = models.CharField(max_length=15)
    email = models.EmailField()
    aadhar_no = models.CharField(max_length=12)
    address = models.CharField(max_length=255)
    Institute_name=models.CharField(max_length=100)
class BookAdmin(admin.ModelAdmin):
    list_display = ('book_no', 'book_name', 'name', 'mobile_no', 'email','aadhar_no','address','Institute_name')
```
2.admin.py
```
from django.contrib import admin
from .models import Book, BookAdmin
admin.site.register(Book, BookAdmin)
```
# OUTPUT
Include the screenshot of your admin page.
![Screenshot 2025-03-21 221246](https://github.com/user-attachments/assets/66245540-75dd-4ee5-9abf-774832ade4b2)
![Screenshot 2025-03-21 220626](https://github.com/user-attachments/assets/dbb82f92-45ad-45df-9cae-a1640f151f08)
![Screenshot 2025-03-21 222155](https://github.com/user-attachments/assets/0f10ddd5-f219-43f1-97e1-b229610a352f)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
