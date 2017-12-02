这是一个用flask做的博客

## 主要功能

- 文章管理：创建，修改，删除文章
- 分类管理：创建，删除分类
- 评论管理：删除，禁用评论
- 页面管理：创建，删除页面
- sitemap功能

## 用法

最好使用 virtualenv 来隔离全局系统环境和局部项目的依赖

1. 配置环境，安装依赖

```
cd CleanBlog
virtualenv venv
source venv/bin/activate
pip install -r requirements.txt
```

2. 创建数据库，设置配置文件

```
CREATE DATABASE person_blog CHARSET=UTF8; 
```

3. 创建数据表

```
python manager.py initdb
```

4. 运行

```
python manager.py runserver
```
