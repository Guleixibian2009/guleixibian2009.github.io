# 从头开始建设GithubPages
--by Guleixibian2009  
![license](https://img.shields.io/github/license/Guleixibian2009/guleixibian2009.github.io)
![GitHub last commit](https://img.shields.io/github/last-commit/Guleixibian2009/guleixibian2009.github.io)  
有人问，这个`github.io`是怎么做出来的？其实很简单，今天我就教大家创建一个`GithubPages(github.io)`页面，分享一下我做网站时的心得。

## 步骤分解
__话不多说，直接上步骤！__
1.加速github，改hosts；   
2.注册github，创建<username>.github.io仓库；<br />
3.创建index.md；<br />
4.创建_config.yml，选择样式；<br />
5.图片外链设置； <br />

## 1.加速

### 1.1 查IP

[Github](https://github.com) 是啥为了节省篇幅我就不讲了,自己去查 [百度百科](https://baike.baidu.com/item/Github/10145341?fr=aladdin) 吧。
不过这东东是国外的，所以我们会需要去加速它。这里推荐一种最安全的方法----查IP。
  

### 1.2 DevSidecar----边车系统

 **小提示：使用此系统可能会造成系统网络配置更变，请小心驾驶**  
 介东西是我某个同学推荐的，具体好不好我也不好说，快是真地快......具体教程请去他的 [Github项目地址](https://github.com/docmirror/dev-sidecar) 。  
 用之前要先安装证书，随后选择默认模式。  

![sidecar1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/sidecar1.png)
![sidecar2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/sidecar2.png)

## 2.基础设置
现在，我们可以做一些基本配置了。

### 2.1 注册Github账号
用Github，没个账号可不行。去官网注册一个账号，步骤如下：  
如图，填写你的邮箱和用户名，应该就好了。

![frontpage](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/frontpage.png)
![email](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/email.png)

我用360大家见谅哈~（尴尬：我注册时不是这样啊？？？）  
不管怎么样了，现在你登录Github，（如果需要验证码就登录一下）大概是这个样子的：  

![myPage](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/myPage.png)

### 2.2 创建一个仓库
为了储存我们的代码，我们需要分配给他一个空间，学名 repository ，意思是仓库。  
如图，点击右上角的 New 按钮，然后会弹出如下界面。

![create1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/create1.png)
![create2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/create2.png)

我们如图勾选，

![create3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/create3.png)

在 `<username>` 处填上你的名字，如果名字是 EdogawaNotFound , 那仓库名就叫  
EdogawaNotFound.GitHub.io 。 

现在你应该有了一个新仓库了。打开你的仓库，应该是这样的：

![repo2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/repo2.png)

现在，你有了自己的仓库，就可以往仓库里放东西了。

## 3.切入正题

### 3.1 勾选Pages

在使用这个功能之前，你要告诉GitHub你要把这个仓库当做网页源码。  
在 Settings 里找到 pages 选项，应该是这样子的：

![settings2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/settings2.png)

把 Source 调成你现有的分支，点击 Save 。  

![settings3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/settings3.png)

### 3.2 重命名README

![change1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/change1.png)

为了githubpages更好的识别你的主页，我们需要更名README。点击那支笔，进入如下界面。

![change2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/change2.png)

红框框内的命称是文件名。我们把他改成 index.md(如果不太对的话......也有可能是我记错了)

![change3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/change3.png)

回来大概是这样的。  
你的网站，如果已经Publish，应该叫做`<username>.github.io>`
现在访问你的网站，如果可以访问，恭喜你，你已经成功了！  
但是网站的默认文本是对githubPages功能的介绍。这样的网站，也许对于别人来说没有意义。  
所以，为了让你的网站看起来更加高级亿点点，我们就要开始写文章了。
使用GitHubpages功能时，你并不需要会写HTML，只需要写文章就行了。 而在GithubPages功能里，我们写文章的方法是写Markdown。  
等等，为什么我觉得我的界面太难看了呢？？？(￣ε(#￣)☆╰╮(￣▽￣///))
让我们给自己的网站换个样式。  
不过，如果你想现在学习Markdown了。我另写了一篇文章， [传送门](https://guleixibian2009.github.io/Code/Markdown/01/) 。  

### 3.3 换个样式

一个网站，也许最重要的不是文章的内容，而是他的主页--它的门面，而一个“光鲜靓丽”的主页则是一个很好的选择。  
GithubPages已经给你提供好了一些样式，我们可以直接用。  
转到刚刚那个Settings/Pages,不过这次点ThemeChooser。

![settings3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/settings3.png)

在这个界面，你可以选择一个你喜欢的样式（Theme）。

![theme1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/theme1.png)

在这里面我选了一个Cayman（简约大气）。

![theme2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/theme2.png)

不管你选了哪个，有没有发现你的网站好看多了呢？ 

### 3.4 _config.yml
不知道细心的你有没有发现，你的仓库里面多了一个`_config.yml`文件（千万不要删！）
打开这个文件，你会发现里面有一行文字：
```yml
theme: jekyll-theme-cayman
```
这个`theme`就指的是样式。`jekyll-theme`指的是GithubPages默认给你使用jekyll渲染网站界面。  
在这个文件里你可以调整你的网站的标题，仔细看！

![Title](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/Title.png)

其实很简单，只要往下面添加一行就可以啦！
```yml
title: My Website~
```
你，都学废了吗？

## 4.404页面

最后，如果你碰到了什么问题，欢迎到 [GitHub](https://github.com/Guleixibian2009/guleixibian2009.github.io/issues/2) 评论！  
下一篇（预告）：[GitHubpages高级教程](https://guleixibian2009.github.io/Code/Github/02)！  

