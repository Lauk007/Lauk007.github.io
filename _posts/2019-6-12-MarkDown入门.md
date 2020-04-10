---
layout:     post   				    
title:    MarkDown  				 
subtitle:  MarkDown认识与入门     #副标题
date:       2019-6-12			   	# 时间
author:     Lauk				# 作者
header-img: img/post-bg-2015.jpg 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - 文档工具
---

### 一.标题

 标题是每篇文章都需要也是最常用的格式，在 Markdown 中，如果一段文字被定义为标题，只要在这段文字前加 `#` 号即可。 

![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69492.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1) 

### 二.列表

 熟悉 HTML 的同学肯定知道有序列表与无序列表的区别，在 Markdown 下，列表的显示只需要在文字前加上 `-` 或 `*` 即可变为无序列表，有序列表则直接在文字前加 `1.``2.``3.` 符号要和文字之间加上一个字符的空格。 

 ![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69493.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1) 

### 三.引用

如果你需要引用一小段别处的句子，那么就要用引用的格式。

```
> 例如这样
```

只需要在文本前加入 `>` 这种尖括号（大于号）即可

![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69494.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1) 

### 四.图片与连接

插入链接与插入图片的语法很像，区别在一个 `!`号

插入图片的地址需要图床，这里推荐 [CloudApp](http://www.getcloudapp.com/) 的服务，生成URL地址即可。

![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69495.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1) 

### 五.表格

```
	| Tables        | Are           | Cool  |
	| ------------- |:-------------:| -----:|
	| col 3 is      | right-aligned | $1600 |
	| col 2 is      | centered      |   $12 |
	| zebra stripes | are neat      |    $1 |
```

| Tables        | Are           | Cool  |
| ------------- | ------------- | ----- |
| col 3 is      | right-aligned | $1600 |
| col 2 is      | centered      | $12   |
| zebra stripes | are neat      | $1    |

### 六.代码框

 如果你是个程序猿，需要在文章里优雅的引用代码框，在 Markdown 下实现也非常简单，只需要用两个 ` 把中间的代码包裹起来，如 ``code``。图例：   使用 tab 键 即可缩进

![img](https://cdn.sspai.com/attachment/origin/2014/04/15/69496.jpg?imageView2/2/w/1120/q/90/interlace/1/ignore-error/1) 

### 七.分割线

 分割线的语法只需要另起一行，连续输入三个星号 `***` 即可。 