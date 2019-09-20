# todobackend
Django application
Django application Todobackend is created using django-admin startproject todobackend command:

```
root@vivek-VirtualBox:/home/vivek/Desktop# python -m pip install "django<2"
root@vivek-VirtualBox:/home/vivek/Desktop# django-admin startproject todobackend
```
This creates the project root todobackend folder. It also created a single file called `manage.py`, which is used for management utilities. and also a child folder with the same project name. This folder is referred to as Django Root folder. And it the main python package folder for the application.

Files under the Django Root folder are:

`urls.py` -> Specified how to route the http request based upon the urls of the application.

`settings.py` -> configuration settings of the project.

`wsgi.py` -> provides means for the external web server such as apache or nginx to pipeline http request and response through the application.

In order to activate the virtual environment. Please follow the below instruction. Continuous Delivery tooling and the Project are separated in this project by creating "src" folder and moving Django Root folder contents in the "src" folder.
```
vivek@vivek-VirtualBox:~/Desktop/todobackend# mkdir src

vivek@vivek-VirtualBox:~/Desktop/todobackend# mv {manage.py,todobackend} src

vivek@vivek-VirtualBox:~/Desktop/todobackend#

vivek@vivek-VirtualBox:~/Desktop/todobackend# virtualenv venv

vivek@vivek-VirtualBox:~/Desktop/todobackend# source venv/bin/activate

(venv) vivek@vivek-VirtualBox:~/Desktop/todobackend#

(venv) vivek@vivek-VirtualBox:~/Desktop/todobackend# pip install pip --upgrade

(venv) vivek@vivek-VirtualBox:~/Desktop/todobackend# pip install django

(venv) vivek@vivek-VirtualBox:~/Desktop/todobackend# pip install djangorestframework

(venv) vivek@vivek-VirtualBox:~/Desktop/todobackend# pip install django-cors-headers
```

Navigating to src folder and then "todo" app is created using the below command.

```
(venv) root@vivek-VirtualBox:/home/vivek/Desktop/todobackend# cd src

(venv) root@vivek-VirtualBox:/home/vivek/Desktop/todobackend/src#

(venv) root@vivek-VirtualBox:/home/vivek/Desktop/todobackend/src# python manage.py startapp todo
```
This newly created app and the other reference REST API and CORS headers packages installed.
