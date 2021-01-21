## Deployment
    
To run this project you need the following tools installed:

  - <a href="https://www.python.org/downloads/" target="_blank"> Python3 </a>
  - <a href="https://git-scm.com/" target="_blank"> Git </a>
  - <a href="https://code.visualstudio.com/" target="_blank"> VS Code </a> or a code editor that have a debug tool.

## Local deployment
<details>

<summary>Click to see local deployment instructions</summary>

The following instructions are based on Windows 10 and VS Code editor.

> Instructions:

  I.    Clone the repository from Github.
 ```shell
  git clone <repository name>.git
 ```

  II.  Create a virtual environment with the command:
```shell
 python -m venv env
 
```

  III.   Activate an environment.
```shell
source env/bin/activate
(Ctrl+Shift+P)
Select Interpreter command displays a list of available global environments, virtual environments

Make sure to be always in the env folder and to have the Python environment active.

For more information:
https://code.visualstudio.com/docs/python/environments

```

  IV.   Install all the packages that are required.
```shell
 pip install django
 pip install django-allauth
 pip install djangorestframework
```

  V.   Create a project name.
```shell
  django-admin startproject <project-name> .
```

  VII. Create a new application name.
```shell
  django-admin startapp <app_name>
```

  VIII.   Migrate the models to crete a database template.
```shell
python manage.py migrate
```

  IX.   Create a super user to have access to the admin page.
```shell
python manage.py createsuperuser
```

  X.   Run the application.
```shell
python manage.py runserver

Open the website at http://127.0.0.1:8000
```

</details>