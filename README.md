# WindBlog 博客及博客同步系统
一开始想做是就是自动发布博客到博客园，了解到MetaWeblog协议；后面又想自己搭建博客网站，发现这种Github Pages很好用，这种Jekyll规范的静态网页让我震撼很多，才发现可以这么玩，就想建一个博客网站和同步发布博客的服务系统，WindBlog诞生。


## 静态博客网站
使用的是Github Pages,源码分支：gh-pages（分支必须为这个），访问地址：username.github.io/WindBlog,username改为你的用户名。我用的是马志写的基于jekyll的皮肤（感谢大神）。
### 博客目录
- _posts 文件夹中是我已发布的博客文章。
-  _drafts 文件夹中是我尚未发布的博客文章。
-  _wiki 文件夹中是我已发布的 wiki 页面。
-  images 文件夹中是我的文章和页面里使用的图片。

## 博客同步系统
基于Yii2.0框架，对博客的管理、发布做些自动化。

### 数据库
sql文件放在public.sql,数据库名称jump，用的是PostGresql，
如果你用的事Mysql或者其他数据库，找些工具，例如DBConvert for MySQL & PostgreSQL，做下转换。

### 功能
当前支持 博客园、CSDN、51CTO、sina、163、oscina、chinaunix
- 初始化设置：配置你需要同步博客的账户信息
- 博客操作：添加记录、编辑记录、删除记录、同步操作

复杂度不高，觉得方便吧！

