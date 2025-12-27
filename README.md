# Ex.06 Book Front Cover Page Design
# Date:01.12.2025
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
from django.shortcuts import render

def book_cover(request):
    return render(request, 'cover/book_cover.html')
```
```
from django.contrib import admin
from django.urls import path
from cover import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', views.book_cover, name='home'),
]
```
```
<html>
    <head>
        <meta charset="UTF-8"/>
    <meta http-equiv="X-UA-Compatible" content="IE=edge"/>
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Book Cover</title>
    </head>
    <body>
        <style>
            img{
                margin: 75px;
                border:10px solid gold;
            }
            .book{
                position: relative;
                text-align: center;
            }
            .book-text1{
                position: relative;
                bottom: 450px;
                font-family:'Trebuchet MS', 'Lucida sans Grande','Lucida Sans',Arial, sans-serif;
                font-weight: 1000px;
                font-style: bold;
                font-size: x-large;
                font-display:inherit;
                color:gold;
            }
            .book-text{
                position: relative;
                bottom: 430px;
                color:gold;
                font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'LUcida Sans', Arial, sans-serif;
                font-size: large;
            }
            .book-text2{
                position: relative;
                bottom: 190px;
                color:gold;
                font-family: 'Trebuchet MS','Lucida Sans Unicode', 'Lucida Grande', 'Lucifa Sans', Arial, sans-serif;
                font-weight: 10000px;
                font-size: large;
            }
            .book-text3{
                position: relative;
                bottom: 570px;
            }
            </style>
            <center>
            <div class="book">
                <img src="bgimg.jpg" alt="book" height="650px"width="400px">
            <div class="book-text3">
                 <img src="williampic.jpg" height="200px"width="200px">
                <div class="book-text">
                    <h3>The Most Famous Book</h3>
                </div>
                <div class="book-text1">
                    <h1>HAMLET <br> </h1>
                </div>
                <div class="book-text2">
                    <h2>William Shakespeare</h2>
                </div>
            </div>
        </center>
        </body>
 </html>
```
# OUTPUT:
<img width="1035" height="605" alt="image" src="https://github.com/user-attachments/assets/eaf627ec-97ce-4b0f-92b1-9b258cd9f9f5" />

# RESULT:
The program for designing book front cover page using HTML and CSS is completed successfully.
