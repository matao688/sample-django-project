
<!-- 杨常佑翻译的内容 -->
1.请从预置的 “workspace-postgresql” 开始。
2. 初始化设置将会创建一个数据库，其参数如下：

配置项	         参数值
数据库名称	     dev-project
用户名	         djangodev
密码	         djangodev
切勿在生产环境中使用以上配置，这些配置仅用于开发环境。
<!-- 在新建数据库时，建立成功后再建表username和password  -->
<!-- 杨常佑翻译的内容 -->


<!--赵毅需要翻译的内容-->

    工作区运行的要求
    下面是我搭建一个新网站所需要的基础配置操作
       PostgresSQL 数据库部署
       Python部署
         DJango 框架
       Node JS部署
         React 框架
      支持Heroku ready部署

<!--赵毅需要翻译的内容-->


<<<<<<< HEAD


<!-- 卢奕成翻译的内容 -->
### 6. 更新 `settings.py` 中的数据库配置

为了在开发过程中将 Django 项目连接到本地的 PostgreSQL 数据库，请按如下方式更新 `settings.py` 文件中的 `DATABASES` 配置部分：

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',  # 使用 PostgreSQL 作为数据库后端
        'NAME': 'dev-project',                                # PostgreSQL 数据库名称
        'USER': 'djangodev',                                  # 数据库用户名
        'PASSWORD': 'djangodev',                              # 数据库密码
        'HOST': 'localhost',                                  # PostgreSQL 所在主机
        'PORT': '',                                           # 留空表示使用默认的 PostgreSQL 端口（5432）
    }
}
此配置适用于本地开发环境。
注意： 在生产环境中，不应将用户名和密码等敏感信息硬编码在 settings.py 中，而应通过环境变量或专门的配置管理系统来管理


<!-- 卢奕成翻译的内容 -->
=======
<!--黄国铭需要翻译的内容-->

完成项目还需的步骤
现在环境已准备好启动一个 Django 应用程序和 React 应用程序。

1.前往 GitHub 并创建一个新的代码仓库。
2.使用命令行（CLI）执行 git remote set-url origin git@github.com:<用户名>/<新仓库> 或 git remote set-url origin https://github.com/<用户名>/<新仓库>
3.使用命令行（CLI）执行 django-admin startproject <项目名称> .
4.使用命令行（CLI）执行 django-admin startapp <应用名称>
5.切换目录并运行 npx create-react-app <React应用名称>
6.更新 Django 的设置

<!--黄国铭需要翻译的内容-->
>>>>>>> ea4794631cc5552c2b9d5c780cd51084fce98378
