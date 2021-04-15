# 从头开始建设GithubPages
--by Guleixibian2009

有人问，这个`github.io`是怎么做出来的？其实很简单，今天我就教大家创建一个`GithubPages(github.io)`页面。

## 步骤分解
1.加速github，改hosts；  
2.安装SublimeText3、GitForWindows、Typora；  
3.注册github，连接Git，配置SSH密钥；  
4.讲解基本Git语法，创建<username>.github.io仓库；<br />
5.使用Typora创建index.md,Sublime修改_config.yml；<br />
6.Markdown初级语法（有外链）；<br />
7.图片外链设置； <br />

## 1.加速

### 1.1 查IP

[Github](https://github.com)是啥为了节省篇幅我就不讲了,自己去查[百度百科](https://baike.baidu.com/item/Github/10145341?fr=aladdin)吧。
不过这东东是国外的，所以我们会需要去加速它。这里推荐一种最安全的方法----查IP。
首先在`C:\Windows\System32\drivers\etc`找到`hosts`文件。这个文件里在没有改动的情况下只有几行注释，忽略即可。
现在我们到[Ipaddress](https://www.ipaddress.com)查下面三个网址的IP：
> 1. github.com 这是主站
> 2. assets-cdn.github.com 动态资源
> 3. github.global.ssl.fastly.net 静态资源

我现在查询如下：

> 140.82.114.4 github.com  
> 185.199.108.153 assets-cdn.github.com  
> 185.199.109.153 assets-cdn.github.com  
> 185.199.110.153 assets-cdn.github.com  
> 185.199.111.153 assets-cdn.github.com  
> 199.232.69.194 github.global.ssl.fastly.net  

按照这样的格式输入到 hosts 文件里，再访问[Github](github.com)应该就很快了！  
**小提示：平时只用查主站的IP就好了，其他的基本不会变~**  

### 1.2 DevSidecar----边车系统

 **小提示：使用此系统可能会造成系统网络配置更变，请小心驾驶**  
 介东西是我某个同学推荐的，具体好不好我也不好说，快是真的快......具体教程请去他的[Github项目地址]()。

## 2.安装配套软件
1.将文件上传到GitHub，我们会用到Git；  
2.编写主页面，我们需要写`Markdown`，我推荐Typora；  
3.修改其他文件，除了记事本我们也可以用SublimeText3。  
安装这些软件一般都是一路Yes，会英文的同学可以仔细看看。安装包见附件。  

## 3.账号设置
现在，我们可以做一些基本配置了。


最后更新：2021-04-12
