# Markdown基本语法
--by guleixibian  
![license](https://img.shields.io/github/license/guleixibian/guleixibian.github.io)
![GitHub last commit](https://img.shields.io/github/last-commit/guleixibian/guleixibian.github.io)  
在很多博客、论坛，包括GithubPages(参见[这篇文章](https://guleixibian.github.io/GPS/)) 里都有大量运用到一种叫做Markdown的文本语言。不管你是在创建自己的网站、写文章，一般平台都需要写Markdown。如果你想学习Markdown，你算是来对地方了！

## 0. Markdown 是什么？
>Markdown是一种轻量级标记语言，创始人为约翰·格鲁伯(英语:John Gruber)。  
>它允许人们使用易读易写的纯文本格式编写文档，然后转换成有效的XHTML(或者HTML)文档。这种语言吸收了很多在电子邮件中已有的纯文本标记的特性。  
>由于Markdown的轻量化、易读易写特性，并且对于图片，图表、数学式都有支持，目前许多网站都广泛使用Markdown来撰写帮助文档或是用于论坛上发表消息。如GitHub、OpenStreetMap 、SourceForge、简书等，甚至还能被使用来撰写电子书。    
>（摘自百度百科）  

___

## 1. 标题
标题在文章中随处可见（包括这篇）。

### 1.1 像HTML一样写标题
在HTML里，标题分六级：

```HTML
<h1>This is an H1</h1>
<h2>This is an H1</h2>
<h3>This is an H1</h3>
...
```

相对应的，Markdown标题也分六级。

```markdown
# This is an H1  
## This is an H2  
...  
###### This is an H6  
```

就像你看到的那样，每层标题就是几个**\#**。

### 1.2 Markdown专属标题
不过，在Markdown中表示标题也可以用一种特殊的方式。

```Markdown

This is an H1
=============

This is an H2
-------------

```
不过它本身只支持2种标题（即大、小标题）。

___
## 2. 文字样式语法
在Markdown中，文字可以是*斜体*、**粗体**、***粗斜体***,~~删除线~~，<u>下划线</u>。

### 2.1 基本样式
- 斜体用一个\*包围，就像` *这是斜体* `，显示出来就是 *这是斜体* 
- 粗体用两个\*包围，就像` **这是粗体** `，显示出来就是 **这是粗体**
- 粗斜体用三个\*包围，就像` ***这是粗斜体*** `，显示出来就是 ***这是粗斜体***
- 删除线用两个\~包围，就像` ~~这是删除线~~ `，显示出来就是 ~~这是删除线~~

### 2.2 某些来自HTML的样式

> 由于Markdown可以直接转换成HTML（在百科里说过了），所以所有（应该是）HTML标签都可以在Markdown中使用。（惊不惊喜？学过HTML的朋友福利大放送！）

#### 2.2.1 瞎划线（下划线）
下划线是用HTML实现的，在HTML里下划线是` <u> `,所以语法就是` <u>这是下划线</u> `,显示出来就是<u>这是下划线</u>  

#### 2.2.2 颜色
如果<font color=green> 你 </font>需要给文字调 <font color=red> 颜色 </font> ，可以用 ` <font> ` 标签，语法为
```HTML
<font color=red> Some text </font>
```

### 2.3 脚注
这是一个脚注 [^1] 。脚注的语法是：
```Markdown
TextTextText [^name] TextTextText
```

___
## 3. 链接与图片

### 3.1 链接
文章中的“链接”指“超链接”。 [这是一个超链接实例](https://guleixibian.github.io/) ，它指向我的主页。  
链接的语法为 

```Markdown
[Name](Place) 
```

### 3.2 图片
图片的语法和链接很相似，只是在 \[Name\]\(Place\) 之前加上一个 \! (记住都是英文标点！！！),如

```Markdown
![Name](Place "替代名")
```

___
## 4. 列表
在Markdown中，列表分两种：有序的，和无序的（还有 “待办事项” ！他属于无序列表）。

### 4.1 有序列表
有序列表，就像  
```Markdown
1. 第一个元素  
2. 第二个元素  
3. 第三个元素
```
在Markdown中，直接打 1. 就会出现一个有序列表。当然， i. a. 甚至不从头开始也可以：



### 4.2 无序列表
无序列表的原理和有序列表一样，不过不以 1. 打头，而是：

```Markdown
- 第一种方式
- 第一种方式
```

```Markdown
+ 第二种方式
+ 第二种方式
```

```Markdown
* 第三种方式
* 第三种方式
```
显示出来都是
- 无序列表
- 无序列表

### 4.3 To do list
通过无序列表我们还可以创建一个任务表（To do list），如下：

- [x]  No.1
- [ ]  No.2
- [x]  No.3

语法如下：
```Markdown
[x] No.1
[ ] No.2
[x] No.3
```
其中 [x] 表示“已完成”，[] 表示“未完成”。

### 4.4 合并列表
谁说列表不能重合？

- 这是一个无序列表  
    1. 这是一个有序列表  
    2. 这是一个有序列表   
- 这是一开始的无序列表  
    - [x] 这是一个To do list。  
    - [ ] 这也是。   
- 这还是某个无序列表 

---
## 注释
以下是注释内容：  

[^1]: 这是一个脚注示例。


___
__THE END__ 谢谢你的阅读~
