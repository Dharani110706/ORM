# Ex02 Django ORM Web Application
## Date:12/05/2025 

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
models.py

from django.db import models
from django.contrib import admin
class Customer (models.Model):
    cid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class CustomerAdmin(admin.ModelAdmin):
    list_display=('cid','name','salary',age','email')

admin.py

from django.contrib import admin
from .models import Customer,CustomerAdmin
admin.site.register(Customer,CustomerAdmin)

```

## OUTPUT

![alt text](<Screenshot 2025-05-12 143015.png>)

Include the screenshot of your admin page.


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
