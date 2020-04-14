---
layout:     post   				    
title:    javascript复习笔记  				 
subtitle:  javascript复习笔记     #副标题
date:       2020-4-14			   	# 时间
author:     Lauk				# 作者
header-img: img/post-bg-2015.webp 	#这篇文章标题背景图片
catalog: true 						# 是否归档
tags:								#标签
    - 前端 - javascript
---

### 一.JavaScript中的数据类型

 **javascript中一共有六种数据类型。parseInt()强转整数、parseFloat()强转浮点数** 

 graph TD 函数类型[函数类型] -->|一共六种| B(s bo fun<br />) B -->|布尔型| C[boolean] B -->|字符串型| D[string] B -->|对象型|E[object] B -->|函数型|F[function] B -->|未定义|G[undefined] B -->|整数型|H[number] 

### 二.获取元素节点

#### 1. **使用ID获取标签节点** 

 `document.getElementById('元素ID');` 

#### 2. **获取name标签** 

 `document.getElementsByName('元素名称');` 

#### 3. **用标签获取指定标签** 

 `document.getElementsByTagName('标签名称');` 

#### 4.使用类名获取元素

 `document.getElementsByClassName('类名');` 

#### 5.改变标签的值

```
var i = document.getElemenrById('bqid');
i.style.background = 'red';
```

### 三.在元素中插入内容

#### 1.在元素中插入文本内容

```
var i = document.getElementById('span');
i.innerText += '一段文本';
```

#### 2. **在元素中插入HTML内容** 

```
var i = document.getElementById('span');
i.innerHTML += ‘<h1></h1>';
```

#### 3.标签生成及添加

```
//生成一个a标签
var i = document.createElement('a');
document.createTextNode('一段文本');        //生成一个字符串
i.href  = 'http://www.baidu.com';
var b = document.body;
b.appendChild(i);   //将A标签添加到Body中
```

#### 4.判断元素节点还是属性节点

```
/**
  *如果是2 则为属性节点
  *如果是1 则为元素节点
  *如果是3 则为文本节点
*/
var a = document.createElement('div');              //生成一个DIV的元素
var b = document.createElement('一段文本');       //生成一段文本内容
a.nodeType == 1;    //元素节点
a.nodeType == 3;    //文本节点
```

#### 5.获取及设置元素属性

```
//注：火狐不支持以下方法
var i = document.getElementById('a');
var o =i.getAttribute('href');   //获取元素属性
i.setAttribute('href','http://www.qq.com');   //设置元素属性
i.removeAttribute('href');      //移除I元素中的href属性
```

#### 6.获取当前元素的上一个、下一个及父级

```
var i = document.getElementById('a');
i.nextElementSibling;       //上一个元素节点
i.previousElementSibling;   //下一个元素节点
var t = i.parentElement;            //父级元素节点
t.childNodes                    //t下所有子级的元素节点
```

#### 7.鼠标移入移出事件

```
//先获取想要触发事件的元素
var a = document.body;
//设置鼠标移入的事件
a.onmousemove = function(ee){
    alert('你的鼠标压到我了');
    //同时也可以改变样式
    ee.target.style.background = 'red';
}
//设置鼠标移出的事件
a.onmouseout = function(eq){
    //和鼠标移入一样设置
    alert('你的鼠标移走了');
    eq.target.style.background = '';
}
```

#### 8.事件合集

```
var div = document.getElementById('div');
div.onclick = function (e){...代码段} //e中的target代表了当前点击的这个元素。e.target
div.onmousemove = function(e){...代码段}  //鼠标在DIV上的移动事件
div.onmouseout = function(e){...代码段}    //鼠标移出DIV的事件
div.onblur = function (e){...代码段}           //失去焦点事件
div.focus()                                         //使DIV获取焦点
div.onkeydown = function(e){e.key}//在DIV元素中按下某键前的事件：e.key为按下的键值
div.onkeypress = function(e){...代码段}    //在DIV元素中某件松开前的事件
```

