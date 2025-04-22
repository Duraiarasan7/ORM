# Ex02 Django ORM Web Application
## Date: 22.04.25

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/f8b45b00-cfd6-486f-975c-2b7040e120a2)


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
from.models import Loan,LoanAdmin
admin.site.register(Loan,LoanAdmin)

models.py

from django.db import models

# Create your models here.
from django.contrib import admin
class Loan(models.Model):
   loan_id=models.IntegerField(primary_key=True)
   loan_type=models.CharField(max_length=30)
   loan_amount=models.FloatField()
   cust_acntno=models.IntegerField()
   cust_name=models.CharField(max_length=50)

class LoanAdmin(admin.ModelAdmin):
    list_display=('loan_id','loan_type','loan_amount','cust_acntno','cust_name')
```



## OUTPUT

![image](https://github.com/user-attachments/assets/26581b31-daf6-4529-8e36-6e6419387fb3)
![image](https://github.com/user-attachments/assets/0ef56c65-c1bf-421a-8944-6216e0fbfc3d)




## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
