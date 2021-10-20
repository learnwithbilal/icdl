# Welcome to bilal company <br>![logo photo](https://github.com/Osama-alaranji/icdl/blob/main/logo.png)
## 1 -Learn how to setup python and install django <br><br>
### 1- Go to python website to download python<br><br>
![python download](https://github.com/Osama-alaranji/icdl/blob/main/1.png)
![python download](https://github.com/Osama-alaranji/icdl/blob/main/2.png)
<br><br><br>
> **_NOTE:_** 
> - If you have windows 7 download 3.8 python version
> .<br>
### 2- Run the setup and check this box <br>
- [x] Add python 3.10 to PATH <br><br>
![python download](https://github.com/Osama-alaranji/icdl/blob/main/3.png)<br>
### 3- After setup open cmd and write `python`   <br><br>
![python download](https://github.com/Osama-alaranji/icdl/blob/main/5.png)
### congratulations , now setup django   <br>
### 1- Open cmd and write `pip install django`  <br>
![django](https://github.com/Osama-alaranji/icdl/blob/main/6.png)<br>
### 2- Write `django-admin startproject Project_Name` to begin your first project 
![django](https://github.com/Osama-alaranji/icdl/blob/main/7.png)<br>
### 3- Now we have two files in project folder 
![django](https://github.com/Osama-alaranji/icdl/blob/main/8.png)<br>
## 2- how to run localhost on your computer
### 1- In the same folder write `python manage.py runserver` to run the server
![django](https://github.com/Osama-alaranji/icdl/blob/main/9.png)<br>
### 2- Now the server is running go to the browser and write `http://127.0.0.1:8000/`
![django](https://github.com/Osama-alaranji/icdl/blob/main/10.png)<br>
![django](https://github.com/Osama-alaranji/icdl/blob/main/11.png)<br>
### 3- Go back to cmd and click `ctrl + c ` to close server
<br><br><br>
## 3- Create apps and link it with our project 
### 1- Open cmd and write  `django-admin startapp AppName`
![django](https://github.com/Osama-alaranji/icdl/blob/main/12.png)<br>
### 2- open visual code in same folder
![django](https://github.com/Osama-alaranji/icdl/blob/main/13.png)<br>
### 3- Go to app folder to the view file and write what you want for user interface
![python download](https://github.com/Osama-alaranji/icdl/blob/main/14.png)<br>
### 4- In app folder add new file `urls.py`
![django](https://github.com/Osama-alaranji/icdl/blob/main/16.png)<br>
### and write inside him
```python
from . import views   # . mean same folder 
from django.urls import path

urlpatterns = [
    path("", views.index, name="index"), # path("url-name" , views.function , name="name-for-you")
    ]
```
### 6- Go to project folder to settings file and write your appname in INSTALLED_APPS<br> to install your app
![django](https://github.com/Osama-alaranji/icdl/blob/main/15.png)<br>
### 7- In project folder go to urls file to make url for your app 
```python
from django.urls import path , include #just add , include 
```
```python
 path('AppName/', include("AppName.urls")) #just add this path
```
![django](https://github.com/Osama-alaranji/icdl/blob/main/17.png)<br>

### 8- Run the server again 
![django](https://github.com/Osama-alaranji/icdl/blob/main/9.png)<br>
### 9- Go to the browser and write `http://127.0.0.1:8000/AppName/`
![django](https://github.com/Osama-alaranji/icdl/blob/main/18.png)<br>
### 10- Finish ----------------------------------------------------
