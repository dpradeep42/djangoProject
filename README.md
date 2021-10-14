# Django
## Installation of required softwares or tools
### You can choose any one of the below mentioned methods
### 1. Standalone Installation of Python.
Go to [Python](https://www.python.org/) and download the compaitable one and install the same on your machine. _While installing Python make sure you're not skipping PIP in it_.

To start with

Install Django using PIP
      
    pip install django

To create a Django project use the below syntax

django-admin startproject project_name 

	django-admin startproject DjangoBasic

After we’ve created the Django Project we’ll have the project created in the respective directory and we can see the folder with the project name and also a few files created like 
-	__init.py__

&emsp;&emsp;It’s a blank python file. But with the naming convention of this file python will treat this directory as a package.

-	settings.py

&emsp;&emsp;This is where you’ll save all your project settings.

-	urls.py

&emsp;&emsp;This is a Python script that will store all the URL patterns for your project. Basically, the different pages of your web application.

-	wsgi.py

&emsp;&emsp;This is a Python script that acts as the Web Server Gateway Interface. It will later on help us deploy our web app to production.

-	manage.py

&emsp;&emsp;This is a Python script that we will use a lot. It will be associates with many commands as we build our web app!
