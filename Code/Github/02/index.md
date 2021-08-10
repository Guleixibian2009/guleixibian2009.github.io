# 3个小妙招加速你的GitHub，妈妈再也不怕你的GitHub上不去啦！
--by Guleixibian2009  
![license](https://img.shields.io/github/license/Guleixibian2009/guleixibian2009.github.io)
![GitHub last commit](https://img.shields.io/github/last-commit/Guleixibian2009/guleixibian2009.github.io)  
想必大家都知道Github是一个极佳的云端代码储存、交流平台，同时你也可以简单粗暴地把它当作云盘或者服务器。
但在众多优点之中，有一个问题却一直深深地困扰着我，那就是GitHub实在太！慢！啦！  
在我头几次用github的时候，我几乎根本上不去，不过以前不过是下载一些搜索到的小工具啥的。
但现在不一样了。我开始做网站，开始天天（也许不是天天）更新，每一次都等待几十分钟的加载时间（白天还好），
简直就是浪费生命。相信大家都有同感吧！  
于是，我就整理了下面3种方法，给大家节约“生命”。

## 0.目录

- 方法一：修改`Host`，其实更加浪费生命  
- 方法二：改链接，做镜像，世界变得更加美好  
- 方法三：装“边车”，速度嗖嗖嗖直窜3秒！  

## 1. 我有大把时间，我要改hosts！
好吧，如果你真的这么无聊，那我就讲一讲吧......  
首先在`C:\Windows\System32\drivers\etc`找到`hosts`文件。如果你以前没用过，那可能需要打开权限。（如下图）

![hosts1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/hosts1.png)
![hosts2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/hosts2.png)
![hosts3](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/hosts3.png)

用记事本打开，这个文件里在没有改动的情况下只有几行注释，忽略即可。  
现在我们到 [Ipaddress](https://www.ipaddress.com) 查下面三个网址的IP：

> GitHub.com 这是主站  
> assets-cdn.GitHub.com 动态资源  
> GitHub.global.ssl.fastly.net 静态资源

我现在查询如下：

> 140.82.114.4 GitHub.com  
> 185.199.108.153 assets-cdn.GitHub.com  
> 185.199.109.153 assets-cdn.GitHub.com  
> 185.199.110.153 assets-cdn.GitHub.com  
> 185.199.111.153 assets-cdn.GitHub.com  
> 199.232.69.194 GitHub.global.ssl.fastly.net

按照这样的格式输入到 hosts 文件里，再访问 [Github](https://github.com/) 应该就很快了！  
**小提示：每次只用查主站的IP就好了，其他的基本不会变~**  

## 2. 我只用GitHub下载程序，不使用其他功能！

## 3. 我天天要用GitHub，给个靠谱的方法！

在Gitee上有一个项目，叫做`@docmirror/DevSidecar`，中文名
**小提示：使用此系统可能会造成系统网络配置更变，请小心驾驶**  
介东西是我某个同学推荐的，具体好不好我也不好说，快是真地快......具体教程请去他的 [Github项目地址](https://github.com/docmirror/dev-sidecar) 。  
用之前要先安装证书，随后选择默认模式。

![sidecar1](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/sidecar1.png)
![sidecar2](https://guleixibian2009.github.io/Source/Pics/Code/Github/01/sidecar2.png)

