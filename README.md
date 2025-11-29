# Ex01 Django ORM Web Application
## Date: 27/11/2025

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 5 Car 

## PROGRAM
```
models.py
from django.db import models
from django.contrib import admin
# Create your models here.
class Student(models.Model):
    student_name = models.CharField(max_length=20, help_text="Enter Student Name")
    age = models.IntegerField(help_text="Enter age between 18 to 22")
    dob = models.DateField()
    reg_no = models.IntegerField(help_text="Enter the Register Number")
<<<<<<< HEAD
=======

class StudentAdmin(admin.ModelAdmin):
    list_display = ['student_name', 'age', 'dob', 'reg_no']
admin.py
from django.contrib import admin
from .models import Student, StudentAdmin
# Register your models here.
admin.site.register(Student, StudentAdmin)
```
## OUTPUT
<img width="1918" height="987" alt="Screenshot 2025-11-28 161422" src="https://github.com/user-attachments/assets/88a71d7d-91c4-42d6-b772-77db60cead19" />
<img width="1918" height="1020" alt="Screenshot 2025-11-28 161339" src="https://github.com/user-attachments/assets/6e84303e-a6ab-44f1-938f-253df8d789b0" />

>>>>>>> a4194590b1a64226c17f5618931b2efa6cdab670

class StudentAdmin(admin.ModelAdmin):
    list_display = ['student_name', 'age', 'dob', 'reg_no']

admin.py
from django.contrib import admin
from .models import Student, StudentAdmin
# Register your models here.
admin.site.register(Student, StudentAdmin)
```
## OUTPUT
![alt text](<Screenshot 2025-11-28 161422.png>)
![alt text](<Screenshot 2025-11-28 161339.png>)
## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
