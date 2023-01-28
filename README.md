# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS
STEP 1:

An Django application is created inside dataproject folder.

STEP 2:

A python program is written to create a table to store and retrieve data.

STEP 3:

The table is created with 6 fields in which the username field is made as PrimaryKey.

STEP 4:

Then the project files migrated. A superuser is also created.

STEP 5:

Now the server side program is executed .

STEP 6:

The admin page of our website is accessed using username and password.

STEP 7:

Records are added and saved in the table inside the database.

## PROGRAM
```
from django.db import models
from django.contrib import admin
# Create your models here.

class Student(models.Model):
    referencenumber = models.CharField(max_length=8, primary_key=True ,help_text="Your Reference Number")
    name = models.CharField(max_length=100)
    age = models.IntegerField()
    email = models.EmailField()

class StudentAdmin(admin.ModelAdmin):
    list_display = ('referencenumber','name','age','email')
```

Include your code here

## OUTPUT
![3](https://user-images.githubusercontent.com/114382660/215249599-a61f1433-caa9-4a5d-9b44-c14111cbc3ca.png)




## RESULT
Thus a Django application is successfully developed to store and retrieve data from a database using Object Relational Mapping(ORM).
