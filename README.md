[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/sizhky/sample-django-project/)

# Pre-built Workspace for My Development
I needed a workspace I could use to start projects from in Gitpod and I didn't find a existing example done the way I wanted. Please keep in mind that my development is all done as a hobby.

## Requirements for the workspace

These are my basic setup items I use when building a new website.
这些是我在建立新网站时通常使用的基础设置：<卢奕成>
* PostgresSQL database
* Python
    * Django
* Node JS
    * React
* Heroku ready
    支持部署到 Heroku  <卢奕成>
## Steps run by gitpod

1. Start with prebuilt "workspace-postgresql"
1. Setups will create a database with the following:
    Item | parameter
    -----|----------
    Database Name | dev-project
    Username | djangodev
    Password | djangodev

** DO NOT USE ** the above settings in a production project. These are only to be used for development.
## Gitpod 启动时执行的步骤   <卢奕成>
1.从预构建的 workspace-postgresql 镜像开始                       <卢奕成>

2.自动设置数据库，具体参数如下：                                 <卢奕成>
    项目  |	 参数                                               <卢奕成>
    -----|----------
    数据库名称	dev-project                                     <卢奕成>
    用户名	djangodev                                           <卢奕成>
    密码	djangodev                                           <卢奕成>

  **  注意：**  以上数据库设置仅用于开发环境，不要在生产环境中使用。     <卢奕成>

## Steps left at finish project
The enviroment is now ready to start a Django app and React App.
1. Go to github and create a new repository.
1. CLI `git remote set-url origin git@github.com:<username>/<new_repo>` or `git remote set-url origin https://github.com/<username>/<new_repo`
1. CLI `django-admin startproject <project name> .`
1. CLI `django-admin startapp <app name>`
1. Change directory <project name> and run `npx create-react-app <react app name>`
1. Update settings for Django


## 项目完成后需手动完成的步骤                       <卢奕成>
环境已经搭建完成，现在可以开始开发 Django 应用和 React 应用了：    

1.去 GitHub 创建一个新仓库       
2.命令行执行                     
    git remote set-url origin git@github.com:<你的用户名>/<新仓库名>或git remote set-url origin https://github.com/<你的用户名>/<新仓库名>                             
3.使用base命令行创建 Django 项目   
    django-admin startproject <项目名称> .           
4.使用命令行创建 Django 应用
    django-admin startapp <应用名称>
5.进入项目目录后，创建 React 应用
    npx create-react-app <react 应用名称>

6.更新 Django 配置文件（settings.py）中的数据库设置
    DATABASES = {
        'default': {
            'ENGINE': 'django.db.backends.postgresql_psycopg2',
            'NAME': 'dev-project',
            'USER': 'djangodev',
            'PASSWORD': 'djangodev',
            'HOST': 'localhost',
            'PORT': '',
        }
    }


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

##参考资料
    Gitpod 官方文档
    https://www.gitpod.io/docs/

    Coding for Entrepreneurs 的 Reactify Django 项目

    https://codingforentrepreneurs.com/projects/reactify-django

    https://github.com/codingforentrepreneurs/Reactify-Django
