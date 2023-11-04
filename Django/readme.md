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
    



