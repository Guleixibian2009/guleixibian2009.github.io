# 一些新鲜出炉的Python代码！
![license](https://img.shields.io/github/license/guleixibian/guleixibian.github.io)
![GitHub last commit](https://img.shields.io/github/last-commit/guleixibian/guleixibian.github.io)  
--by guleixibian  

我一直喜欢Python这种语言，我也经常写Python的程序，今天就给大家共享一下吧！  

> 小知识#1  
>
> Python是一种跨平台的计算机程序设计语言。 是一个高层次的结合了解释性、编译性、互动性和面向对象的脚本语言。
> 最初被设计用于编写自动化脚本(shell)，随着版本的不断更新和语言新功能的添加，越多被用于独立的、大型项目的开发。  
>
> 如果你不知道Python的话，就去 [Python官网](https://www.python.org/about/gettingstarted/) 看看吧。

**好。现在言归正传，正式开始！！！**

## 1. 打出大写字母

直接上代码（just because 它太简单了...）！  

```python
string = 'AbCdEfG'
for letter in string:
	if letter.isupper():
		print(letter)、
```

敢说大部分人都写得出来这种程序吧，不过我还是把它写上了。不过我一开始还真没相信 `for letter in string`这一行......[尴尬]  

*现在讲解代码！* 首先我们定义了一个字符串(string就是字符串)，内容是一些字母，既有大写又有小写。然后用一个for循环，遍历每一个字母，再检测他是不是大写(`if letter.isupper()`)。如果字母大写就打印出来。  

![Run1](https://guleixibian.github.io/Source/Pics/Code/Python/01/run1.png)  

看吧，他回复了你ACEG。  

> 小知识#2  
>
> 我们不仅仅可以用`letter.isupper()`来判定一个字母是否是大写，也可以用`letter.islower()`来判定一个字母是否是小写。当然，`"hello".upper()`可以将"hello"这个字符串大写，`"HELLO".lower()` 可以将 "HELLO" 变成小写。

## 2.凯撒密码

下面这段代码可以将任何字符串加密，*但是它特别容易被破解*。同时，这段代码也没有任何难度，除了马上要登场的`chr()`和`ord()`。（我给打个1星吧，前面那个0.5星[调皮]）
