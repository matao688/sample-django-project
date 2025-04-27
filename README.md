# Gitpod Ready-to-Code Workspace | Gitpod 即开即用开发环境

[![Gitpod ready-to-code](https://img.shields.io/badge/Gitpod-ready--to--code-blue?logo=gitpod)](https://gitpod.io/#https://github.com/sizhky/sample-django-project/)

---

## 📁 Table of Contents | 目录                      <卢奕成>
- [✨ About | 项目介绍](#-about--项目介绍)
- [⚙️ Workspace Setup | 工作区设置要求](#️-workspace-setup--工作区设置要求)
- [🛠️ Gitpod 自动执行步骤 | Gitpod 自动运行步骤](#️-gitpod-自动执行步骤--gitpod-自动运行步骤)
- [🚀 After Setup | 完成基础配置后要做的事](#-after-setup--完成基础配置后要做的事)
- [📚 References | 参考资料](#-references--参考资料)

---

## ✨ About | 项目介绍                                          <卢奕成>
I needed a Gitpod workspace that matches my development habits. I couldn't find an existing one that fit, so I built this myself.  
> 我需要一个符合自己开发习惯的 Gitpod 工作区示例，但没有找到合适的，于是自己搭建了一个。  
> (【注：开发仅作为个人兴趣爱好】)

---

## ⚙️ Workspace Setup | 工作区设置要求                          <卢奕成>
These are the basic tools and services I always set up for new projects.  
> 以下是我每次新建项目时必备的基础环境：

- PostgreSQL database | PostgreSQL 数据库
- Python  
  - Django
- Node.js  
  - React
- Heroku ready | 支持 Heroku 部署

---

## 🛠️ Gitpod 自动执行步骤 | Gitpod 自动运行步骤                     <卢奕成>

1. Start from the prebuilt image: **`workspace-postgresql`**  
   > 从预构建镜像 `workspace-postgresql` 启动
2. Automatically create a database with the following settings:  
   > 自动创建数据库，参数如下：

| Item 项目       | Parameter 参数 |
|-----------------|----------------|
| Database Name   | dev-project     |
| Username        | djangodev       |
| Password        | djangodev       |

> ⚠️ **Do NOT use these settings in production! Only for development!**  
> ⚠️ **注意：以上设置仅限开发环境使用，不可用于生产环境！**

---

## 🚀 After Setup | 完成基础配置后要做的事          <卢奕成>

Once Gitpod finishes setting up, you can start Django and React projects:  
> Gitpod 初始化完成后，可以开始开发 Django 和 React 项目：                 <卢奕成>

1. Create a new GitHub repository | 创建一个新的 GitHub 仓库            <卢奕成>
2. Set Git remote URL in CLI | 通过命令行设置 Git 远程地址              <卢奕成>

```bash
git remote set-url origin git@github.com:<your-username>/<your-new-repo>.git
# or
git remote set-url origin https://github.com/<your-username>/<your-new-repo>.git
```

3. Start a Django project | 创建 Django 项目                    <卢奕成>

```bash
django-admin startproject <project-name> .
```

4. Start a Django app | 创建 Django 应用                        <卢奕成>

```bash
django-admin startapp <app-name>
```

5. Create a React app inside project directory | 在项目目录下创建 React 应用    <卢奕成>

```bash
npx create-react-app <react-app-name>                                       <卢奕成>
```

6. Update `settings.py` database settings | 更新 `settings.py` 中的数据库配置：         <卢奕成>

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',
        'NAME': 'dev-project',
        'USER': 'djangodev',
        'PASSWORD': 'djangodev',
        'HOST': 'localhost',
        'PORT': '',
    }
}                                                               <卢奕成>

```

---

## 📚 References | 参考资料<卢奕成>

- [Gitpod Documentation | Gitpod 官方文档](https://www.gitpod.io/docs/)<卢奕成>
- [Reactify Django (Coding for Entrepreneurs) | Reactify Django 教程](https://codingforentrepreneurs.com/projects/reactify-django)<卢奕成>
- [Reactify Django GitHub Repo](https://github.com/codingforentrepreneurs/Reactify-Django)<卢奕成>

---

