# GithubPages——简单易上手的网站制作
--by guleixibian2009  

![license](https://img.shields.io/github/license/guleixibian2009/guleixibian2009.github.io)
![GitHub last commit](https://img.shields.io/github/last-commit/guleixibian2009/guleixibian2009.github.io)  

今天我就来教大家创建一个`GithubPages(github.io)`页面，分享一下我做网站时的心得。
其实我一直想要做网站。在6个月前（2021年2月），我开始看着 [W3School](https://www.w3school.com.cn/)
上的教程，用SublimeText写HTML。
但写了一两个月后，我突然想起来一件事。  
大概在一年前，我有个同学给我推荐了一个录屏软件（不过我忘了叫什么了）。他给了我一个网址，然后，
__我看到了一个熟悉的东西__————这个网址里有github的字样。于是，我搜（百）索（度）了一会子，
然后搜到好多有关“用Github.io创作个人博客”的文章，没想到做网站也可以这么简单。

## 步骤分解
__话不多说，直接上步骤！__    
1.注册github，创建<username>.github.io仓库；  
2.创建index.md；  
3.创建_config.yml，选择样式；  
4.404页面；

___
## 1.基础设置
想必大家看完上文已经知道了我们的网站依托于 [Github](https://github.com/) 。
身为程序员，大家应该都知道GitHub是什么吧。如果你不知道的话，可以看看 [这里](https://guleixibian2009.github.io/Code/Github/) 
或者查询 [百度百科](https://baike.baidu.com/item/Github) 。

### 1.1 注册Github账号
如果你没用过Github，就去官网注册一个账号，步骤如下：  
如图，填写你的邮箱和用户名，应该就好了。

![frontpage](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/frontpage.png)
![email](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/email.png)

（尴尬：我注册时不是这样啊？？？）  
登录Github可能会需要验证码。登录一下注册时的邮箱，你会收到Github（`noreply@github.com`）的邮件，比如说：

![Authentication](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/Authentication.png)

### 1.2 创建一个仓库
为了储存我们的代码，我们需要分配给他一个空间，学名 repository ，意思是仓库。  
如图，点击右上角的 New 按钮，然后会弹出如下界面。

![create1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/create1.png)
![create2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/create2.png)

我们如图勾选，

![create3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/create3.png)

在 `<username>` 处填上你的名字，如果名字是 EdogawaNotFound , 那仓库名就叫  
EdogawaNotFound.GitHub.io 。 

现在你应该有了一个新仓库了。有了自己的仓库，就可以往仓库里放东西了。

___
## 2.切入正题

### 2.1 勾选Pages

在使用这个功能之前，你要告诉GitHub你要把这个仓库当做网页源码。  
在 Settings 里找到 pages 选项，应该是这样子的：

![settings2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/settings2.png)

把 Source 调成你现有的分支，点击 Save 。  

![settings3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/settings3.png)

### 2.2 重命名README

![change1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/change1.png)

为了GithubPages更好的识别你的主页，我们需要新建一个index.md。你可以保留你的README不动，没有关系。

![New1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/New1.png)

点击 + 按钮，选择Create New File，然后进入如下界面：

![New2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/New2.png)

在输入框里输入index.md。Index指索引。你将会在这个新文件里写主页。

![New3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/New3.png)

点击Commit New Changes。

![change3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/change3.png)

回来大概是这样的。  
你的网站，如果已经Publish，应该叫做`<username>.github.io>`
现在访问你的网站，如果可以访问，恭喜你，你已经成功了！   
所以，为了让你的网站看起来更加高级亿点点，我们就要开始写文章了。
使用GitHubpages功能时，你并不需要会写HTML，只需要写文章就行了。 而在GithubPages功能里，我们写文章的方法是写Markdown。  
等等，为什么我觉得我的界面太难看了呢？？？(￣ε(#￣)☆╰╮(￣▽￣///))
让我们给自己的网站换个样式。  
不过，如果你想现在学习Markdown了。我另写了一篇文章， [传送门](https://guleixibian2009.github.io/Code/Markdown/01/) 。  

### 2.3 换个样式

一个网站，也许最重要的不是文章的内容，而是他的主页--它的门面，而一个“光鲜靓丽”的主页则是一个很好的选择。  
GithubPages已经给你提供好了一些样式，我们可以直接用。  
转到刚刚那个Settings/Pages,不过这次点ThemeChooser。

![settings3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/settings3.png)

在这个界面，你可以选择一个你喜欢的样式（Theme）。

![theme1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/theme1.png)

在这里面我选了一个Cayman（简约大气）。

![theme2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/theme2.png)

不管你选了哪个，有没有发现你的网站好看多了呢？ 
不过，他会自动填充你的index.md。网站的默认文本是对githubPages功能的介绍。这样的网站，也许对于别人来说没有意义。
(不过如果没有的话......也许是因为你先创建了文件再选择样式，其实也没事)  

### 2.4 _config.yml
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

___
## 3.404页面
在访问你的网站时，别人总有输错网址的时候。Github其实有自带的404，像这样：

![404](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/404.png)

不过这个灰色的404实在是不好看，那么，我就有了一个疑问：我能不能自己定制

最后，如果你碰到了什么问题，欢迎到 [GitHub](https://github.com/guleixibian2009/guleixibian2009.github.io/issues/2) 评论！  
下一篇（预告）：[GitHubpages高级教程](https://guleixibian2009.github.io/Code/Github/02)！  

___
__THE END__ 谢谢你的阅读~