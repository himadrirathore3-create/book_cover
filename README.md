# Ex.05 Book Front Cover Page Design
# Date:5/12/2025
# AIM:
To design a book front cover page using HTML and CSS.

# DESIGN STEPS:
## Step 1:
Create a Django Admin project.

## Step 2:
Create an app in the Django interface.

## Step 3:
Create a folder named 'static' in the app folder.

## Step 4:
Create a new HTML file in the static folder.

## Step 5:
Write the HTML code with relevant CSS properties.

## Step 6:
Choose the appropriate style and color scheme.

## Step 7:
Insert the images in their appropriate places.

## Step 8:
Publish the website in the LocalHost.

# PROGRAM:
```
urls.py

from django.contrib import admin
from django.urls import path
from myapp import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('',views.cover,name='home')
]
```
```
views.py

from django.shortcuts import render
def cover(request):
    return render (request,'cover.html')
```
```
{% load static %}
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>BOOK COVER</title>

 
  <link rel="stylesheet" href="{% static 'book.css' %}">
</head>
<body>

  <div class="book-container">

    <div class="title">WALK INTO THE SHADOW</div>
    <div class="subtitle">The shifty shadows that transforms world</div>

    <span class="edition"><strong>ORIGINAL EDITION</strong></span>
    <hr class="top">
    <hr class="bottom">

    <span class="author">BENEDICT JULIUS</span>

    <img src="{% static 'bc.jpg' %}" alt="Book Cover" class="book-cover">
    <div class="inner-border"></div>

  </div>

</body>
</html>
```

# OUTPUT:
![alt text](<Screenshot 2025-12-18 212717.png>)
# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
