# Django
First practice project of full-stact web app development using Django framework.

## Getting started with empty project folder
Conda is used here to create virtual environment because of the necessity to manage
various Python versions locally.
Poetry is used to easily manage package dependencies.

### Create virtual environment using conda (download and install Anaconda)
To make the app lightweight, consider only adding the bare minimum of python packages
```bash
conda create --name {myenv} python==3.10 --no-default-packages
```

### Check that the conda environment has been created successfully
```bash
conda env list
```

### Activate the newly created conda virtual environment
```bash
conda activate {myenv}
```

### Initialise poetry (follow this for poetry installation https://python-poetry.org/docs/)
```bash
poetry init
```
Enter Yes for everything

### Add Django using poetry
```bash
poetry add Django
```

### Create Django project
Notice the `.` at the end is important to create the project in the current directory. 
```bash
django-admin startproject django_firstproject .
```

### Create Django app
```bash
python manage.py startapp firstapp
```

### Perform migrations to create necessary database tables
```bash
python manage.py makemigrations
```
```bash
python manage.py migrate
```

### Start a development server to host the app
```bash
python manage.py runserver
```

### Check that your Django app is setup correctly
http://localhost:8000/

