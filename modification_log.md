<!-- 杨常佑 翻译作业 -->
在进行翻译作业时候，使用AI有以下几点：

1. 翻译时，需要根据英文原文进行翻译，而不是直接翻译为中文。所以在我们使用Ai工具的时候就得确保有中英文的对照。

2. 翻译时，请使用中文，并使用中文注释。在进行术语词汇表的查找时先对其进行翻译，然后再进行术语词汇表的查找。
<!-- 杨常佑 翻译作业 -->



<!-- 全俊召 翻译作业 -->
在进行翻译作业时候，使用AI有以下几点：

1. 仓库操作

- 仓库地址相关：了解了在本地查看 Git 仓库远程地址的命令 git remote -v；还学习到从 GitHub API 获取仓库地址的方法，以及在 CMD 中通过 git remote -v 查看本地仓库远程地址、用 curl 结合 GitHub API 获取仓库地址的操作 。

- 仓库删除：明确了在 GitHub 网页端删除仓库的具体流程，包括登录账号、进入仓库设置、在危险区域确认删除等步骤。

2. Git 账号密码与 SSH 密钥设置

- 账号密码设置：掌握了使用 HTTPS 协议时，通过 git config --global credential.helper 相关命令临时或长期存储账号密码；同时也了解了手动设置 Git 提交时用户名和邮箱的命令。

- SSH 密钥获取与配置：学习了生成 SSH 密钥的命令，如 ssh-keygen -t ed25519 -C "your_email@example.com"；知晓了将 SSH 密钥添加到 SSH 代理、复制公钥到 GitHub 账户的详细操作步骤。

3. 连接报错解决

- 报错信息：针对 fatal: unable to access... 这类连接 GitHub 仓库失败的报错，AI 从网络连接、防火墙和安全软件、代理设置、DNS 配置、GitHub 服务器状态等多个角度分析原因。

- 解决方法：给出了检查网络连通性（如 ping 命令）、排查代理设置（查看和清除代理）、临时关闭防火墙或配置规则、更换 DNS 服务器、查看 GitHub 状态页面等具体解决措施。

4.英语翻译优化
- 对英语叫ai根据关于计算机优化英文
<!-- 全俊召 翻译作业 -->



<!--赵毅的翻译ai修改记录-->

    在使用ai进行翻译作业时，要先把所需要翻译的内容复制下来，去ai粘贴，然后提问ai，让ai翻译所需要翻译的内容。翻译成功后，看着ai翻译出来的内容，进行近义翻译，而不能直接照搬ai翻译出来的，要自己通过思考和分析去翻译作业，从而更好的提高英语水平。
    
    ai翻译中把一些英文翻成了中文，但是一些固定的代码词就没有进行修改，例如python这些固有的英文，因而这样则是直接按照原来的字母写就好了
    
<!--赵毅的翻译ai修改记录-->
    
<!--卢奕成的翻译流程修改记录-->
 更新 settings.py 中的数据库配置（操作流程）
以下是在开发环境中配置 PostgreSQL 数据库连接的详细操作步骤：

步骤 1：确保已安装 PostgreSQL
前往 PostgreSQL 官网 下载并安装适用于你系统的版本
安装过程中设置一个数据库用户（如：djangodev）和数据库（如：dev-project）；
可使用图形界面工具如 pgAdmin 来管理数据库。

步骤 2：安装 Django 的 PostgreSQL 驱动
在你的虚拟环境中运行以下命令安装 psycopg2：
bash
复制
编辑
pip install psycopg2-binary
⚠️ psycopg2-binary 是推荐用于开发的版本。部署到生产环境时请改用 psycopg2。

步骤 3：修改 settings.py 中的数据库配置
打开 Django 项目中的 settings.py 文件，找到 DATABASES 配置部分，修改为如下内容：

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql_psycopg2',  # 使用 PostgreSQL 作为数据库后端
        'NAME': 'dev-project',                                # 数据库名称
        'USER': 'djangodev',                                  # 数据库用户名
        'PASSWORD': 'djangodev',                              # 用户密码
        'HOST': 'localhost',                                  # 数据库主机地址（本地）
        'PORT': '',                                           # 留空则默认使用 5432 端口
    }
}
步骤 4：运行数据库迁移命令
确保数据库已经创建，然后运行以下命令以应用 Django 的模型迁移：
python manage.py makemigrations
python manage.py migrate
步骤 5：启动开发服务器测试连接
python manage.py runserver
如果没有数据库连接错误，即说明配置成功。
 温馨提示：
在生产环境中不要将数据库用户名、密码等敏感信息直接写入 settings.py 文件中。建议使用环境变量、.env 文件或 Django 的 django-environ 等工具进行安全管理。
<!--卢奕成的翻译流程修改记录-->