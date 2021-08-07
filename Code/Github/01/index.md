# 从头开始建设GithubPages
--by Guleixibian2009  
![license](https://img.shields.io/github/license/Guleixibian2009/guleixibian2009.github.io)
![Last Update](https://img.shields.io/badge/LatestUpdate-06.21-brightgreen)  
有人问，这个`github.io`是怎么做出来的？其实很简单，今天我就教大家创建一个`GithubPages(github.io)`页面。  
PS：这个教程用Windows10 64位系统编写，适合Win7及以上。

## 步骤分解
1.加速github，改hosts；   
2.注册github，创建<username>.github.io仓库；<br />
3.创建index.md；<br />
4.Markdown初级语法（有外链）；<br />
5.图片外链设置； <br />

## 1.加速

### 1.1 查IP

[Github](https://github.com) 是啥为了节省篇幅我就不讲了,自己去查 [百度百科](https://baike.baidu.com/item/Github/10145341?fr=aladdin) 吧。
不过这东东是国外的，所以我们会需要去加速它。这里推荐一种最安全的方法----查IP。
首先在`C:\Windows\System32\drivers\etc`找到`hosts`文件。如果你以前没用过，那可能需要打开权限。（如下图）

![hosts1](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/hosts1.png)
![hosts2](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/hosts2.png)
![hosts3](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/hosts3.png)

用记事本打开，这个文件里在没有改动的情况下只有几行注释，忽略即可。  
现在我们到 [Ipaddress](https://www.ipaddress.com) 查下面三个网址的IP：  

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

按照这样的格式输入到 hosts 文件里，再访问 [Github](https://github.com/) 应该就很快了！  
**小提示：每次只用查主站的IP就好了，其他的基本不会变~**  

### 1.2 DevSidecar----边车系统

 **小提示：使用此系统可能会造成系统网络配置更变，请小心驾驶**  
 介东西是我某个同学推荐的，具体好不好我也不好说，快是真的快......具体教程请去他的 [Github项目地址](https://github.com/docmirror/dev-sidecar) 。  
 用之前要先安装证书，随后选择默认模式。  

![sidecar1](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/sidecar1.png)
![sidecar2](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/sidecar2.png)



## 2.基础设置
现在，我们可以做一些基本配置了。

### 2.1 注册Github账号
用Github，没个账号可不行。去官网注册一个账号，步骤如下：  
如图，填写你的邮箱和用户名，应该就好了。

![frontpage](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/frontpage.png)
![email](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/email.png)

我用360大家见谅哈~（尴尬：我注册时不是这样啊？？？）  
不管怎么样了，现在你登录Github，（如果需要验证码就登录一下）大概是这个样子的：  

![myPage](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/myPage.png)

### 2.2 创建一个仓库
为了储存我们的代码，我们需要分配给他一个空间，学名 repository ，意思是仓库。  
如图，点击右上角的 New 按钮，然后会弹出如下界面。

![create1](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/create1.png)
![create2](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/create2.png)

我们如图勾选，


![create3](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/create3.png)

在 <username> 处填上你的名字，如果名字是 EdogawaNotFound , 那仓库名就叫  
EdogawaNotFound.github.io 。 

现在你应该有了一个新仓库了。打开你的仓库，应该是这样的：

![repo2](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/repo2.png)

现在，你有了自己的仓库，就可以往仓库里放东西了。

## 3.主页搭建
是网页就得有个页面吧。使用GitHubpages功能时，你并不需要会写HTML，只需要写文章就行了。  

### 3.1 勾选Pages

在使用这个功能之前，你要告诉GitHub你要把这个仓库当做网页源码。  
在 Settings 里找到 pages 选项，应该是这样子的：

![settings2](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/settings2.png)

把 Source 调成你现有的分支，点击 Save 。  

![settings3](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/settings3.png)


### 3.2 编辑主页
现在你访问你的网站，大概是这样的：

![your1](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/your1.png)

（为什么标题是TEST？因为这是我的网页下的一个分支，你的页面一开始应该有一大堆文字）   
现在，你说你想增加一点东西，怎么办呢？    
在GithubPages功能里，我们写文章的方法是写Markdown。  
不过，在学习它之前，我们要先做一点小小的改变。  

![change1](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/change1.png)

为了githubpages更好的识别你的主页，我们需要更名README。点击那支笔，进入如下界面。

![change2](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/change2.png)

红框框内的命称是文件名。我们把他改成 index.md

![change3](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/change3.png)

回来大概是这样的。  
现在我们可以学Markdown了。我另写了一篇文章，在  
<https://guleixibian2009.github.io/Code/MD/ST/>。  

### 3.3 换个样式

不管你的主页现在写了什么，我们都想让他变好看点。GithubPages已经给你提供好了一些样式，我们可以直接用。  
转到刚刚那个Settings/Pages,不过这次点ThemeChooser。

![settings3](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/settings3.png)

点进去大概是这样的：

![theme1](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/theme1.png)

我选了一个Cayman。

![theme2](https://guleixibian2009.github.io/Sourse/Pics/Code/Github/#1/theme2.png)

现在样式也有了，你的界面基本上也就好了！ 

## 4. 图片外链
这里最后给大家一个小技巧。由于很多人的页面上想放图片，将图片保存到本地又没用，我们把他保存到GitHub上。  
（待会再写啦啦啦啦~）  

最后，如果你碰到了什么问题，欢迎到 [GitHub](https://github.com/Guleixibian2009/guleixibian2009.github.io/issues/2) 评论！  
下一篇（预告）：[GitHubpages高级教程](https://guleixibian2009.github.io/Code/Github/#2)！  

最后更新：2021-06-20
