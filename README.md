# Django
## Installation of required softwares or tools
### You can choose any one of the below mentioned methods
### 1. Standalone Installation of Python.
Go to [Python](https://www.python.org/) and download the compaitable one and install the same on your machine. 

_While installing Python make sure you're not skipping PIP in it_.

To start with

Install Django using PIP
      
    pip install django

To create a Django project use the below syntax

django-admin startproject project_name 

	django-admin startproject DjangoBasic

After we’ve created the Django Project we’ll have the project created in the respective directory and we can see the folder with the project name and also a few files created like 

![alt text](https://github.com/dpradeep42/djangoProject/blob/main/images/project_overview.png)

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

Now to run and check the project which we’ve created we’ll use the below command from the project directory.
	
	python manage.py runserver

after running the above command we’ll see something like below.
```
C:\Users\dpradeepkumar\Django\djangoProject\DjangoBasic>python manage.py runserver
Watching for file changes with StatReloader
Performing system checks...

System check identified no issues (0 silenced).

You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.
October 14, 2021 - 11:49:05
Django version 3.2.8, using settings 'DjangoBasic.settings'
Starting development server at http://127.0.0.1:8000/
Quit the server with CTRL-BREAK.
```
Now we can see the project is running at http://127.0.0.1:8000/

![alt text](https://github.com/dpradeep42/djangoProject/blob/main/images/project_running.png)

After running the project we can see that 
```
You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.
```