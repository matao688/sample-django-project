[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/sizhky/sample-django-project/)

# Pre-built Workspace for My Development
I needed a workspace I could use to start projects from in Gitpod and I didn't find a existing example done the way I wanted. Please keep in mind that my development is all done as a hobby.

## Requirements for the workspace123123123
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
## Steps Remaining to Finish the Project
1.The development environment is now fully configured and ready for initiating a Django application and a React application. Here are the subsequent steps:

2.Navigate to GitHub and create a new repository.
In the Command Line Interface (CLI), use one of the following commands to set the origin URL of your local Git repository according to your preference. If you are using SSH authentication, use: git remote set-url origin git@github.com:<username>/<new_repo>. If you prefer using HTTPS, use: git remote set-url origin https://github.com/<username>/<new_repo>.

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


