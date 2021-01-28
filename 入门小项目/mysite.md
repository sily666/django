#### 1. 安装

查看电脑是否安装django：`pip show django`

#### 2. 创建django项目

+ 打开cmd或者powershell，切换到要创建项目的文件路径下： `cd .\Desktop\`(tab键可以自动补全路径)
+ 创建项目：`django-admin startproject mysite`
+ 将路径切换到项目下：`cd .\mysite\`，输入` code .`命令可以用**vscode**将项目自动打开

![image-20210127220905559](C:\Users\pansu\Desktop\django\1.assets\image-20210127220905559.png)

此时的项目文件结构：

![image-20210127221038516](C:\Users\pansu\Desktop\django\1.assets\image-20210127221038516.png)

然后可以在vscode终端启动项目：`python manage.py runserver`

<img src="C:\Users\pansu\Desktop\django\1.assets\image-20210127221514881.png" alt="image-20210127221514881" style="zoom: 33%;" />

#### 3. 配置路由urls

+ 创建app：`python manage.py startapp mob`
+ 在**settings.py**中添加**mob**这个app
+ 在mysite下的**urls.py**中添加mob对应的**路由**，同时引入**include**方法
+ 在mob文件下创建**urls.py**文件

![image-20210127222140035](C:\Users\pansu\Desktop\django\1.assets\image-20210127222140035.png)

![image-20210127222350841](C:\Users\pansu\Desktop\django\1.assets\image-20210127222350841.png)

![image-20210127222527038](C:\Users\pansu\Desktop\django\1.assets\image-20210127222527038.png)

![image-20210127222907858](C:\Users\pansu\Desktop\django\1.assets\image-20210127222907858.png)

#### 4. 展示html页面

+ 设定路由跳转的**path**，引入views里面的方法
+ 定义**views.py**中对应的**方法**
+ 在mysite的**setting.py**中添加模板文件。
+ 创建**templates**文件夹，编写html页面

![image-20210127223752393](C:\Users\pansu\Desktop\django\1.assets\image-20210127223752393.png)

![image-20210127223927919](C:\Users\pansu\Desktop\django\1.assets\image-20210127223927919.png)

![image-20210128175354384](C:\Users\pansu\Desktop\django\1.assets\image-20210128175354384.png)

![image-20210127224053562](C:\Users\pansu\Desktop\django\1.assets\image-20210127224053562.png)

#### 5. 创建公共html模板

+ 创建**base.html**作为模板文件，直接从bootstrap复制初学者模板https://v4.bootcss.com/docs/getting-started/introduction/
+ 将**home.html**文件引入到**base.html**文件中

![image-20210128185322217](C:\Users\pansu\Desktop\django\1.assets\image-20210128185322217.png)

![image-20210128201943259](C:\Users\pansu\Desktop\django\1.assets\image-20210128201943259.png)

#### 6. 展示导航信息

+ 直接到bootstrap中复制一段navbar代码 https://v4.bootcss.com/docs/components/navbar/



#### 7. 接口地址

 https://api.github.com/

http://jsonplaceholder.typicode.com/



#### 8. 接口请求和解析

+ 在view.py中获得api，通过render第三个参数传递给home.html

![image-20210128211056915](C:\Users\pansu\Desktop\django\1.assets\image-20210128211056915.png)

此外，需要下载requests模块

![image-20210128210736861](C:\Users\pansu\Desktop\django\1.assets\image-20210128210736861.png)



#### 9. 展示数据信息

![image-20210128212600455](C:\Users\pansu\Desktop\django\1.assets\image-20210128212600455.png)

#### 10. 搜索界面跳转

+ 添加url
+ 创建对应的方法和页面
+ 搜索跳转表单

![image-20210128213340242](C:\Users\pansu\Desktop\django\1.assets\image-20210128213340242.png)

![image-20210128220825388](C:\Users\pansu\Desktop\django\1.assets\image-20210128220825388.png)

![image-20210128220849728](C:\Users\pansu\Desktop\django\1.assets\image-20210128220849728.png)

![image-20210128220939579](C:\Users\pansu\Desktop\django\1.assets\image-20210128220939579.png)