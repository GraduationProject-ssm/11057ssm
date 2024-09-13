# [首页查询更多项目](https://github.com/GraduationProject-ssm) 包安装运行


# 11057ssm校园点餐系统

![picture](https://raw.githubusercontent.com/GraduationProject-springboot/.github/main/img/wx.png)

### 点击播放视频 ▼
[![Watch the video](https://i.sstatic.net/Vp2cE.png)](https://www.bilibili.com/video/BV1Kp48e9EtU?p=101)


# 系统概述
进过系统的分析后，就开始记性系统的设计，系统设计包含总体设计和详细设计。总体设计只是一个大体的设计，经过了总体设计，我们能够划分出系统的一些东西，例如文件、文档、数据等。而且我们通过总体设计，大致可以划分出了程序的模块，以及功能。但是只是一个初步的分类，并没有真正的实现。

整体设计，只是一个初步设计，而且，对于一个项目，我们可以进行多个整体设计，通过对比，包括性能的对比、成本的对比、效益的对比，来最终确定一个最优的设计方案，选择优秀的整体设计可以降低开发成本，增加公司效益，从这一点来讲，整体设计还是非常重要的。

校园点餐系统工作原理图如图4-1所示：

![](/md/blog.012.png)

图4-1 系统工作原理图
## 4.2 系统结构设计
系统架构图属于系统设计阶段，系统架构图只是这个阶段一个产物，系统的总体架构决定了整个系统的模式，是系统的基础。校园点餐系统的整体结构设计如图4-2所示。

![](/md/blog.013.png)

图4-2 系统结构图
## 4.3数据库设计
数据库是计算机信息系统的基础。目前，电脑系统的关键与核心部分就是数据库。数据库开发的优劣对整个系统的质量和速度有着直接影响。
### 4.3.1 数据库设计原则
数据库的概念结构设计采用实体—联系（E-R）模型设计方法。E-R模型法的组成元素有：实体、属性、联系，E-R模型用E-R图表示，是提示用户工作环境中所涉及的事物，属性则是对实体特性的描述。在系统设计当中数据库起着决定性的因素。下面设计出这几个关键实体的实体—关系图。
### 4.3.2 数据库实体
数据模型中的实体（Entity），也称为实例，对应现实世界中可区别于其他对象的“事件”或“事物”。例如，公司中的每个员工，家里中的每个家具。

本系统的E-R图如下图所示：

1、商家信息实体图如图4-3所示：

![](/md/blog.014.png)

`  `图4-3商家信息实体图

2、用户信息实体图如图4-4所示：

![](/md/blog.015.png)

`          `图4-4用户信息实体图

3、菜品信息实体图如图4-5所示：

![](/md/blog.016.png)

`         `图4-5菜品信息实体图

#########

### 4.3.3 数据库表设计
数据库的表信息属于设计的一部分，下面介绍数据库中的各个表的详细信息。

表4-1 allusers表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|username|varchar|50|` `default NULL|
|pwd|varchar|50|` `default NULL|
|cx|varchar|50|` `default NULL|

表4-2 caipinxinxi表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|shangjiabianhao|varchar|50|default NULL|
|shangjiaming|varchar|50|default NULL|
|caixi|varchar|50|default NULL|
|meishimingcheng|varchar|50|default NULL|
|tupian|varchar|50|default NULL|
|danjia|varchar|50|default NULL|
|zhuliao|varchar|50|default NULL|
|fenliang|varchar|50|default NULL|
|meishijieshao|varchar|50|default NULL|

表4-3：shangjia表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|` `int|11|NOT NULL |
|addtime|varchar|50|default NULL|
|shangjiabianhao|varchar|50|default NULL|
|mima|varchar|50|default NULL|
|shangjiaming|varchar|50|default NULL|
|fuzeren|varchar|50|default NULL|
|lianxidianhua|varchar|50|default NULL|
|shangjiadizhi|varchar|50|default NULL|
|yingyezhizhao|varchar|50|default NULL|
|sfsh|varchar|50|default NULL|
|shhf|varchar|50|default NULL|

表4-4 yonghu表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|xuehao|varchar|50|default NULL|
|mima|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
|xingbie|varchar|50|default NULL|
|zhaopian|varchar|50|default NULL|
|yuanxi|varchar|50|default NULL|
|dianhua|varchar|50|default NULL|
|dizhi|varchar|50|default NULL|
|sfsh|varchar|50|default NULL|
|shhf|varchar|50|default NULL|

表4-5 waimaidingdan表

|列名|数据类型|长度|约束|
| :-: | :-: | :-: | :-: |
|id|int|11|NOT NULL|
|addtime|varchar|50|default NULL|
|dingdanbianhao|varchar|50|default NULL|
|shangjiabianhao|varchar|50|default NULL|
|shangjiaming|varchar|50|default NULL|
|meishimingcheng|varchar|50|default NULL|
|caipinfenlei|varchar|50|default NULL|
|xuehao|varchar|50|default NULL|
|xingming|varchar|50|default NULL|
|dianhua|varchar|50|default NULL|
|dizhi|varchar|50|default NULL|
|jiage|varchar|50|default NULL|
|fenliang|varchar|50|default NULL|
|jine|varchar|50|default NULL|
|xiadanshijian|varchar|50|default NULL|
|qucanshijian|varchar|50|default NULL|
|qucanfangshi|varchar|50|default NULL|
|sfsh|varchar|50|default NULL|
|shhf|varchar|50|default NULL|




# 5统详细设计
## 5.1前台首页功能模块
校园点餐系统，在系统首页可以查看首页、菜品信息、外卖订单、新闻资讯、我的、跳转到后台、客服等内容，如图5-1所示。

![](/md/blog.017.png)

图5-1前台首页功能界面图



用户登录，在登录页面可以填写账号、密码等信息进行登录，如图5-2所

示。

![](/md/blog.018.png)

图5-2用户登录界面图
#########
菜品信息，在菜品信息页面通过查看商家编号、商家名、菜系、美食名称、图片、单价、主料、份量、美食介绍等信息进行购买、点我收藏，如图5-3所示。在个人中心页面通过填写学号、姓名、性别、照片、院系、电话、地址、审核回复等信息进行更新信息、退出登录操作，如图5-4所示。

![](/md/blog.019.png)

图5-3菜品信息界面图
#########
![](/md/blog.020.png)

图5-4个人中心界面图

## 5.2管理员功能模块
管理员登录，通过填写用户名、密码进行登录，如图5-5所示。

![](/md/blog.021.png)

图5-5管理员登录界面图

管理员登录进入校园点餐系统可以查看个人中心、用户管理、商家管理、菜系分类管理、菜品信息管理、外卖订单管理、系统管理等信息。

用户管理，在用户管理页面中可以通过查看学号、姓名、性别、照片、院系、电话、地址、是否审核、审核回复等内容进行详情、修改、删除，如图5-6所示。还可以根据需要对商家管理进行详情，修改等详细操作，如图5-7所示。

![](/md/blog.022.png)

图5-6用户管理界面图

![](/md/blog.023.png)

图5-7商家管理界面图

菜系分类管理，在菜系分类管理页面中可以查看菜系等信息，并可根据需要对已有菜系分类管理进行修改或删除等操作，如图5-8所示。

![](/md/blog.024.png)

图5-8菜系分类管理界面图

菜品信息管理，在菜品信息管理页面中可以查看商家编号、商家名、菜系、美食名称、图片、单价、主料、份量、美食介绍等信息，并可根据需要对已有菜品信息管理进行修改或删除等详细操作，如图5-9所示。

![](/md/blog.025.png)

图5-9菜品信息管理界面图

外卖订单管理，在外卖订单管理页面中可以查看订单编号、商家编号、商家名、美食名称、菜品分类、学号、姓名、电话、地址、价格、份量、金额、下单时间、取餐时间、取餐方式、是否审核、审核回复、是否支付等内容，并且根据需要对已有外卖订单管理进行详情，修改或删除等详细操作，如图5-10所示。

![](/md/blog.026.png)

图5-10外卖订单管理界面图

轮播图；该页面为轮播图管理界面。管理员可以在此页面进行首页轮播图的管理，通过新建操作可在轮播图中加入新的图片，还可以对以上传的图片进行修改操作，以及图片的删除操作，如图5-11所示。

![](/md/blog.027.png)

图5-11轮播图管理界面图

美食资讯管理，在美食资讯管理页面中可以查看标题、简介、图片、内容等信息，并且根据需要对已有美食资讯管理进行详情，修改或删除等详细操作，如图5-12所示。

![](/md/blog.028.png)

图5-12美食资讯管理界面图


## 5.3商家功能模块
商家登录进入校园点餐系统可以查看个人中心、菜系分类管理、菜品信息管理、外卖订单管理等内容。

菜系分类管理，在菜系分类管理页面中通过查看菜系等信息，还可以根据需要对菜系分类管理进行修改，如图5-13所示。

![](/md/blog.029.png)

图5-13菜系分类管理界面图

菜品信息管理，在菜品信息管理页面中可以查看商家编号、商家名、菜系、美食名称、图片、单价、主料、份量、美食介绍等信息，并且根据需要对已有菜品信息管理进行查看删除等其他详细操作，如图5-14所示。

![](/md/blog.030.png)

图5-14菜品信息管理界面图
#########
外卖订单管理，在外卖订单管理页面中通过查看订单编号、商家编号、商家名、美食名称、菜品分类、学号、姓名、电话、地址、价格、份量、金额、下单时间、取餐时间、取餐方式、是否审核、审核回复、是否支付等内容进行详情、修改、删除，如图5-15所示。

![](/md/blog.031.png)

图5-15外卖订单管理界面图
#########
## 5.4用户功能模块
用户登录进入校园点餐系统可以查看个人中心、外卖订单管理、我的收藏管理等内容，如图5-16所示。

![](/md/blog.032.png)

图5-16用户功能界面图













