<h1 align="center">Django</h1>

## installation:
* creating a virtual enviroment<br>
we need to create virtual enviroment so that we can isolate our project from all other projects on the system
- windows
    * using python -
    `python -m venv projectone` : this create a virtual environment called projectone
    * activating virtual environment -
        `projectone\Scripts\activate`
    * deactivating a virtual environment: `deactivate`
- linux
    * using python -
    `python -m venv projectone` : this create a virtual environment called projectone
    * activating virtual environment -
        `source project/bin/activate`
    * deactivating a virtual environment: `deactivate`

for more info visit: [here](https://docs.python.org/3/tutorial/venv.html) 

***

After the virtual environment is created and activated we can install django inside the virtual environment by using pip:- 
```
python -m pip install Django
```

- we can verify whether Django is installed by typing this in the terminal: 

    ```
    python -m django --version
    ```
    If this outputs the version number of the currently installed django then everything is installed properly.
***

# Sample project to tryout:
## basic poll application
    An application where people can vote on people and an admin panel where we can add,remove and monitor votes.

### creating project:
Before we start typing the project we need to generate some code for our django project. we can do so using the following command.

```
Django-admin startproject project_name
```
 Make sure to run the command with the virtual environment active. The above command will create a directory named project_name with the necessary files for a django project with the following structure :
    
    project_name/  --> can be renamed, it just considered as a container
    manage.py
    project_name/  --> the root folder of your django project
        __init__.py  --> used to indicate that this directory is a python package
        settings.py  --> confige file for the django project
        urls.py  -->
        asgi.py
        wsgi.py

***
### Development Server
It is a server that comes with every django project. Do not use this server for deployment. we can turn on the server by using the following command.

    python manage.py runserver

make sure to use this command after changing to the directory with the manage.py file. After running the above command you should get an output like this


    (env) D:\github\project-trial\dbmsproject>python manage.py runserver
    Watching for file changes with StatReloader
    Performing system checks...

    System check identified no issues (0 silenced).

    You have 18 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): admin, auth, contenttypes, sessions.
    Run 'python manage.py migrate' to apply them.
    November 25, 2023 - 19:22:35
    Django version 4.2.7, using settings 'dbmsproject.settings'
    Starting development server at http://127.0.0.1:8000/
    Quit the server with CTRL-BREAK.

this means that the server is now live at 127.0.0.1:8000 and can be opened using the provide ip address.


