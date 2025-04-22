# Ex02 Django ORM Web Application
## Date: 21.04.2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![Screenshot 2025-04-22 224545](https://github.com/user-attachments/assets/63a7f16f-1230-45c6-a5ac-1a7cda1e3a2d)


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
class Movie(models.Model):
        Serialno=models.IntegerField(primary_key="sno")
        Name=models.CharField(max_length=10)
        Email=models.EmailField()
        Movie=models.CharField(max_length=30)
        DateTime=models.DateTimeField()
       
class MovieAdmin(admin.ModelAdmin):
         list_display=('Serialno','Name','Phoneno','Email','Movie','DateTime',)

admin.py

from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)
```


## OUTPUT
![Screenshot 2025-04-22 223948](https://github.com/user-attachments/assets/a469d706-f037-49f7-8a5b-ae4a15c192da)


Include the screenshot of your admin page.


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
