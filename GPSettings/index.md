# 从头开始建设GithubPages
--by Guleixibian2009

有人问，这个`github.io`是怎么做出来的？其实很简单，今天我就教大家创建一个`GithubPages(github.io)`页面。  
PS：这个教程用Windows7 64位系统操作，适合Win7以上。

## 步骤分解
1.加速github，改hosts；  
2.安装SublimeText3、GitForWindows、Typora；  
3.注册github，创建<username>.github.io仓库；<br />
4.使用Typora创建index.md,Sublime修改_config.yml；<br />
5.Markdown初级语法（有外链）；<br />
6.图片外链设置； <br />

## 1.加速

### 1.1 查IP

[Github](https://github.com)是啥为了节省篇幅我就不讲了,自己去查[百度百科](https://baike.baidu.com/item/Github/10145341?fr=aladdin)吧。
不过这东东是国外的，所以我们会需要去加速它。这里推荐一种最安全的方法----查IP。
首先在`C:\Windows\System32\drivers\etc`找到`hosts`文件。这个文件里在没有改动的情况下只有几行注释，忽略即可。
现在我们到[Ipaddress](https://www.ipaddress.com)查下面三个网址的IP：
> github.com 这是主站
> assets-cdn.github.com 动态资源
> github.global.ssl.fastly.net 静态资源

我现在查询如下：

> 140.82.114.4 github.com  
> 185.199.108.153 assets-cdn.github.com  
> 185.199.109.153 assets-cdn.github.com  
> 185.199.110.153 assets-cdn.github.com  
> 185.199.111.153 assets-cdn.github.com  
> 199.232.69.194 github.global.ssl.fastly.net  

按照这样的格式输入到 hosts 文件里，再访问[Github](https://github.com/)应该就很快了！  
**小提示：平时只用查主站的IP就好了，其他的基本不会变~**  

### 1.2 DevSidecar----边车系统

 **小提示：使用此系统可能会造成系统网络配置更变，请小心驾驶**  
 介东西是我某个同学推荐的，具体好不好我也不好说，快是真的快......具体教程请去他的[Github项目地址](https://github.com/docmirror/dev-sidecar)。

## 2.安装配套软件

### 2.1 Typora
编写页面，我们需要写Markdown，我推荐Typora。  
这个编辑器支持写完一小段代码你就可以看到它实际上看起来是什么样的。  
Typora官网：<https://typora.io/>

### 2.2 SublimeText3
修改其他文件，比如`_config.yml`，我们用SublimeText3。  
这个软件什么语言都能写，也可以当做简单的文本编辑器用。  
官网：<https://www.sublimetext.com/>  
你甚至可以用他们家的Git命令行，叫做SublimeMerge，比默认的好很多！

安装这俩软件一般都是一路Yes，会英文的同学可以仔细看看。安装包见附件。  

## 3.基础设置
现在，我们可以做一些基本配置了。

### 3.1 注册Github账号
用Github，没个账号可不行。去官网注册一个账号，步骤如下：  
如图，填写你的邮箱和用户名，应该就好了。

![frontpage](https://user-images.githubusercontent.com/79316026/115193983-67a72f00-a11f-11eb-89d1-3de617888508.png)
![email](https://user-images.githubusercontent.com/79316026/115194097-902f2900-a11f-11eb-880b-569584da054a.png)

我用360大家见谅哈~（尴尬：我注册时不是这样啊？？？）  
不管怎么样了，现在你登录Github，（如果需要验证码就登录一下）大概是这个样子的：  

![myPage](https://user-images.githubusercontent.com/79316026/115195072-e781c900-a120-11eb-95da-904cd7917e70.png)

### 3.2 创建一个仓库
为了储存我们的代码，我们需要分配给他一个空间，学名 repository ，意思是仓库。  
如图，点击右上角的 New 按钮，然后会弹出如下界面。

![create1](https://user-images.githubusercontent.com/79316026/115196027-0896e980-a122-11eb-901e-6a78824725c5.png)
![create2](https://user-images.githubusercontent.com/79316026/115196866-f9646b80-a122-11eb-95df-dcde8f73dab7.png)

我们如图勾选，


![create3](https://user-images.githubusercontent.com/79316026/115196875-fb2e2f00-a122-11eb-802b-d81bef30fb85.png)

在 <username> 处填上你的名字，如果名字是 EdogawaNotFound , 那仓库名就叫  
EdogawaNotFound.github.io 。 
README.md 是仓库简介，可以先不选。LISENCE 同理。  
 
现在你应该有了一个新仓库了。打开你的仓库，如果你刚刚什么都没选，那应该是这样的：

![repo1](https://user-images.githubusercontent.com/79316026/115198822-169a3980-a125-11eb-8269-c7ef1d2da45b.png)

当然，如果你选了刚刚那两项，那应该是这样的：

![repo2](https://user-images.githubusercontent.com/79316026/115332591-b6f66980-a1ca-11eb-90f5-7c1bc9ab5899.png)

现在，你有了自己的仓库，就可以往仓库里放东西了。

## 4.主页搭建
是网页就得有个页面吧。使用GitHubpages功能时，你并不需要会写HTML，只需要写文章就行了。  

### 4.1 勾选Pages

在使用这个功能之前，你要告诉GitHub你要把这个仓库当做网页源码。  
在 Settings 里找到 pages 选项，应该是这样子的：
![settings1](https://user-images.githubusercontent.com/79316026/115333421-333d7c80-a1cc-11eb-8dba-20284786fbd9.png)
![settings2](https://user-images.githubusercontent.com/79316026/115333423-346ea980-a1cc-11eb-82cd-0e16f970dd34.png)

### 4.2 编辑主页
像这样，新建一个文件（如图）。

![new1](https://user-images.githubusercontent.com/79316026/115333061-94b11b80-a1cb-11eb-96e8-0a06e10e95b9.png)

点击 




最后更新：2021-04-20
