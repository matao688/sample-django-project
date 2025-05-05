[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/sizhky/sample-django-project/)

# Pre-built Workspace for My Development
I needed a workspace I could use to start projects from in Gitpod and I didn't find a existing example done the way I wanted. Please keep in mind that my development is all done as a hobby.

## Requirements for the workspace123
These are my basic setup items I use when building a new website.

* PostgresSQL database
* Python
    * Django
* Node JS
    * React
* Heroku ready

<!--赵毅负责上面的英文翻译内容-->
<!--工作区运行的要求
    下面是我搭建一个新网站所需要的基础配置操作
       PostgresSQL 数据库部署
       Python部署
         DJango 框架
       Node JS部署
         React 框架
    支持Heroku ready部署-->



## Steps run by gitpod

1. Start with prebuilt "workspace-postgresql"
2. Setups will create a database with the following:
    Item | parameter
    -----|----------
    Database Name | dev-project
    Username | djangodev
    Password | djangodev

** DO NOT USE ** the above settings in a production project. These are only to be used for development.



## Steps left at finish project
The enviroment is now ready to start a Django app and React App.
1. Go to github and create a new repository.
1. CLI `git remote set-url origin git@github.com:<username>/<new_repo>` or `git remote set-url origin https://github.com/<username>/<new_repo`
1. CLI `django-admin startproject <project name> .`
1. CLI `django-admin startapp <app name>`
1. Change directory <project name> and run `npx create-react-app <react app name>`
1. Update settings for Django
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


