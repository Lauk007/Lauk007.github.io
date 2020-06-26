---
layout:     post   				    
title:    JavaScript原型到原型链   				 
subtitle:  JavaScript原型到原型链     #副标题
date:       2020-6-26			   	# 时间
author:     Lauk				# 作者
header-img: img/post-bg-2015.webp 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - JavaScript
---

### 构造函数创建对象

我们先使用构造函数创建一个对象：

```javascript
function Person() {

}
var person = new Person();
person.name = 'Kevin';
console.log(person.name) // Kevin
```

在这个例子中，Person 就是一个构造函数，我们使用 new 创建了一个实例对象 person。

### prototype

每个函数都有一个 prototype 属性，就是我们经常在各种例子中看到的那个 prototype ，比如：

```javascript
function Person() {

}
// 虽然写在注释里，但是你要注意：
// prototype是函数才会有的属性
Person.prototype.name = 'Kevin';
var person1 = new Person();
var person2 = new Person();
console.log(person1.name) // Kevin
console.log(person2.name) // Kevin
```

