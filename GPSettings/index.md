# 从头开始建设GithubPages
--by Guleixibian2009

有人问，这个`github.io`是怎么做出来的？其实很简单，今天我就教大家创建一个GithubPages(github.io)页面。

## 步骤分解
1.加速github，改hosts；  
2.安装SublimeText3、GitForWindows、Typora；  
3.注册github，连接Git，配置SSH密钥；  
4.讲解基本Git语法，创建<username>.github.io仓库；<br />
5.使用Typora创建index.md,Sublime修改_config.yml；<br />
6.Markdown初级语法（有外链）；<br />
7.图片外链设置； <br />

## 1.加速Github
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

按照这样的格式输入到`hosts`文件里，再访问[Github](github.com)应该就很快了！


最后更新：2021-04-12

