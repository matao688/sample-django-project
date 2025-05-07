[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/sizhky/sample-django-project/)

# Pre-built Workspace for My Development
I needed a workspace I could use to start projects from in Gitpod and I didn't find a existing example done the way I wanted. Please keep in mind that my development is all done as a hobby.

<!--赵毅翻译的内容-->

## Requirements for the workspace
These are my basic setup items I use when building a new website.

* PostgresSQL database
* Python
    * Django
* Node JS
    * React
* Heroku ready

<!--赵毅翻译的内容-->









## Steps run by gitpod
<!-- 杨常佑翻译的内容 -->
1. Start with prebuilt "workspace-postgresql"
2. Setups will create a database with the following:
    Item | parameter
    -----|----------
    Database Name | dev-project
    Username | djangodev
    Password | djangodev

** DO NOT USE ** the above settings in a production project. These are only to be used for development.
<!-- 杨常佑翻译的内容-->



<!--全俊召修改---->
## Steps to Finish the Project
The environment is now prepared to start both a Django app and a React app. Here are the subsequent steps to complete the project setup.

First, visit GitHub and create a new repository. This will serve as the remote location to store your project's code.

Next, open the Command Line Interface (CLI). You need to set the origin URL of your local Git repository. You have two options based on your authentication preference. If you're using SSH, run the command git remote set-url origin git@github.com:<username>/<new_repo>. If you prefer HTTPS, use git remote set-url origin https://github.com/<username>/<new_repo>.

After that, in the CLI, create a new Django project in the current directory. Use the command django-admin startproject <project name> ..

Once the Django project is created, create a new Django app within it. In the CLI, run django-admin startapp <app name>.

Now, switch to the directory of the newly - created Django project. You can do this by running cd <project name>. Then, initialize a new React application using the command npx create-react-app <react app name>.

Finally, you need to update the Django settings. Usually, this involves making changes to files like settings.py. You'll integrate the new app, configure static files, and set up any necessary middleware in this step.
<!--全俊召修改---->

##  Update the Database Configuration in `settings.py`
<!--卢奕成修改---->
To connect the Django project to a local PostgreSQL database during development, update the `DATABASES` section in your `settings.py` file as follows:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',  # Use PostgreSQL as the database backend
        'NAME': 'dev-project',                                # Name of the PostgreSQL database
        'USER': 'djangodev',                                  # Database user
        'PASSWORD': 'djangodev',                              # Database password
        'HOST': 'localhost',                                  # Host where PostgreSQL is running
        'PORT': '',                                           # Leave blank to use default PostgreSQL port (5432)
    }
}
This configuration is suitable for local development environments
Note: For production environments, do not hardcode sensitive information like usernames and passwords in settings.py. Instead, use environment variables or a separate configuration management system.       <!--卢奕成修改---->


## References used to build the workspace
* Gitpod docs
    * https://www.gitpod.io/docs/
* Reactify Django by Coding for Entrepreneurs
    * https://codingforentrepreneurs.com/projects/reactify-django
    * https://github.com/codingforentrepreneurs/Reactify-Django


