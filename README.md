# MyBlog
使用Python+Django构建个人博客

## 1、项目准备

### 1.1、必备工具

安装工具包方式

```
pip install [工具名]==[版本号]
如pip install django==2.2
```

python3.8

django2.2

virtualenvwrapper-win

### 1.2、工程创建和配置

#### 1.2.1、github创建项目仓库

+ 点击头像，选择 Your repositories，点击**New**新建一个代码仓库

+ 输入Repository name，如MyBlog

+ Description输入仓库描述：如使用Python+Django编写个人博客

+ 默认选择public，表示开源可供他人查看

+ 初始化仓库三项都勾选
  + Add a README file，增加说明文档，即README.md
  + Add .gitignore，选择要使用的语言，这里选择Python
  + Choose a license，选择许可协议，这里选MIT License 

+ 仓库创建完成

#### 1.2.2、将仓库克隆到本地使用

**下载安装git**

> 下载地址：https://git-scm.com/downloads

**将github仓库克隆到本地**

```
git clone https://github.com/OrentalDragon/MyBlog.git
```

#### 1.2.3、创建个人博客工程

**安装虚拟环境工具**

```
pip install virtualenvwrapper-win
```

**创建虚拟环境**

```
//mkvirtualenv [虚拟环境名] 
mkvirtualenv -p python3 blog
```

**删除虚拟环境**

```
//rmvirtualenv [虚拟环境名]
rmvirtualenv blog
```

**进入虚拟环境**

```
//workon [虚拟环境名]
workon blog
```

**退出虚拟环境**

```
deactivate
```

**进入虚拟环境后，首先安装Django**

```
pip install django==2.2
```

**然后使用虚拟环境在本地仓库下创建工程**

```
django-admin startproject blog
```

**进入创建的工程blog，启动django项目服务器**

```
cd blog
python manage.py runserver
```

**访问http://127.0.0.1:8000/，查看django页面**

显示The install worked successfully! Congratulations!

表示创建完成

**退出Django项目服务器**

cmd启动，最后一行会提示ctrl+break退出。

不过现在的键盘一般没有break键，可以用fn + p或者fn + b来代替，

所以**ctrl + fn + p**或**ctrl + fn + b**退出

```
ctrl + fn + p
或ctrl + fn + b
```

**在github上更新内容**

```
cd ..   						#进入仓库文件夹blog
git add . 						#
git commit -m 'creatproject' 	#创建工程项目
```

