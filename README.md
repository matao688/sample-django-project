[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/sizhky/sample-django-project/)


<!--韦俊的修改的内容-->

# Pre-built Workspace for My Development
I need to look for a pre-configured Gitpod workspace template to quickly launch projects. 
After conducting extensive searches in Gitpod's public areas, community repositories, 
and forums, I still haven't found a template that meets my needs. My software development is purely a personal hobby for learning and exercising creativity.

Technical terms related to computers:workspace、Gitpod、projects、Git

<!--韦俊的修改的内容-->


<!--赵毅翻译的内容-->

## Requirements for the workspace123123123
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


```Python
DATABASE = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'dev-project',
        'USER': 'djangodev',
        'PASSWORD': 'djangodev',
        'HOST': 'localhost',
        'PORT': '',
    }
}

## References used to build the workspace
* Gitpod docs
    * https://www.gitpod.io/docs/
* Reactify Django by Coding for Entrepreneurs
    * https://codingforentrepreneurs.com/projects/reactify-django
    * https://github.com/codingforentrepreneurs/Reactify-Django


