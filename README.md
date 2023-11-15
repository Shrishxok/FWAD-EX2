# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

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
## models.py
from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class Player_Admin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')
## admin.py
from django.contrib import admin
from .models import Player,Player_Admin
admin.site.register(Player,Player_Admin)
## OUTPUT

<img width="835" alt="Screenshot 2023-11-15 at 10 11 49 PM" src="https://github.com/Shrishxok/FWAD-EX2/assets/120294863/97412b99-9262-45d6-a569-1a95094da571">



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
