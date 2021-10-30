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

We can see that <span style="color: green"> DEBUG=True </span>

![alt text](https://github.com/dpradeep42/djangoProject/blob/main/images/debug_true.png)

We can change this option in settings.py file. This functionality enables us to see what are all the errors which are in our application if there were any. But, before going into the production we have Disable this option so that the end users can't see the errors which are in the application.

After running the project we can see that 
```
You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
Run 'python manage.py migrate' to apply them.
```

### What is a migration?
-	A migration allows you to move databases from one design to another, this is also reversible.
-	So you can “migrate” your database
-	We will touch back on this later, for now you can ignore this warning.

For now we can ignore this.

## Creating our first django Application.
### What is Django Project and Django Application
-	A Django Project is a collection of applications and configurations that when combined together will make up the full web application (your complete website running with Django)
-	A Django Application is created to perform a particular functionality for your entire web application. For example you could have a registration app, a polling app, comments app, etc.
-	These Django Apps can then be plugged into other Django Projects, so you can reuse them! (Or use other people’s apps)

Creating Django Application

	Syntax: python manage.py startapp <App Name>


	python manage.py startapp first_app