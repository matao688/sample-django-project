<!-- 杨常佑  术语词汇表 -->
1.Prebuilt "workspace-postgresql": 预构建的“workspace-postgresql”环境。这通常指的是一个已经配置好的开发环境，包含了PostgreSQL数据库。

2.Database Name: 数据库名称。这是数据库的标识符，在例子中是dev-project。

3.Username: 用户名。用于访问数据库的凭证之一，在例子中是djangodev。

4.Password: 密码。与用户名一起用于认证访问数据库的凭证，在例子中也是djangodev。

5.Production project: 生产项目。指正式运行的环境，与开发环境相对。

6.Development: 开发。指软件开发过程中的测试和调试阶段，与生产环境不同。
<!--杨常佑   术词汇表  -->


<!--赵毅的项目术语表-->
    git clone
    git add  
    git commit -m 
    git push
    git pull
    git config --global user.name
    git config --global user.email 

    PostgreSQL是开源关系型数据库，适合复杂数据操作。
    Python+Django提供高效后端开发，内置ORM简化数据库交互。
    Node.js常用于构建轻量后端服务，搭配React实现动态前端界面。
    Heroku为云部署平台，支持快速发布应用，集成上述技术并自动化运维，便于扩展和管理。
<!--赵毅的项目术语表-->



<!-- 卢奕成 术语词汇表 -->
1. `settings.py`: Django 项目的主配置文件，包含数据库、应用、中间件等核心设置。
2. PostgreSQL: 一种开源的关系型数据库管理系统，支持复杂查询和事务处理，适合中大型项目。
3. psycopg2-binary: Django 连接 PostgreSQL 数据库所需的 Python 驱动程序，适用于开发环境。
4. `DATABASES` 配置字典: Django 中用于设置数据库连接参数的配置项，通常写在 `settings.py` 中。
5. ENGINE: 数据库后端引擎设置，指定使用哪种数据库驱动。`django.db.backends.postgresql_psycopg2` 表示使用 PostgreSQL。
6. NAME: 数据库名称。在配置中指定连接的目标数据库，比如 `dev-project`。
7. USER: 数据库用户名。用于连接数据库的身份验证信息，例如 `djangodev`。
8. PASSWORD: 数据库密码。配合用户名一起用于身份验证，例如 `djangodev`。
9. HOST: 数据库主机地址。在本地开发中通常为 `localhost`，表示数据库运行在本机。
10. PORT: 数据库连接端口。如果留空，Django 将默认使用 PostgreSQL 的标准端口 5432。
11. 开发环境（Development Environment）: 用于编写、调试、测试代码的环境，通常数据库配置会使用本地信息。
12. 生产环境（Production Environment）: 实际对外提供服务的运行环境，配置应更安全，敏感信息不应明文写入代码中。
13. 环境变量（Environment Variables）: 用于在不同环境中动态注入配置信息的一种方式，常用于安全地传递数据库用户名、密码等敏感信息。
14. 数据迁移（Migration）: Django 中用于将模型（Models）中的更改同步到数据库结构的过程，命令包括 `makemigrations` 和 `migrate`。
15. `runserver`: Django 提供的开发用服务器启动命令，用于本地运行项目进行测试和调试。
<!-- 卢奕成 术语词汇表 -->

<!--叶正艺的项目术语表-->

## 开发框架相关

| 英文术语          | 中文对照             | 对应文件       | 具体位置                     |
|-------------------|----------------------|----------------|------------------------------|
| ASGI             | 异步服务器网关接口   | `asgi.py`      | 文件顶部注释和代码实现       |
| WSGI             | Web服务器网关接口    | `wsgi.py`      | 文件顶部注释和代码实现       |
| Middleware       | 中间件               | `settings.py`  | `MIDDLEWARE` 配置项          |
| ALLOWED_HOSTS    | 允许的主机           | `settings.py`  | `ALLOWED_HOSTS = []`         |
| DEBUG            | 调试模式             | `settings.py`  | `DEBUG = True`               |


## 数据库相关

| 英文术语             | 中文对照          | 对应文件       | 具体位  置                                   |
|----------------------|-------------------|----------------|--------------------------------------------|
| SQLite              | SQLite数据库      | `settings.py`  | `DATABASES` 默认配置                       |
| ENGINE (SQLite)     | SQLite引擎        | `settings.py`  | `'ENGINE': 'django.db.backends.sqlite3'`   |










<!--叶正艺的项目术语表-->