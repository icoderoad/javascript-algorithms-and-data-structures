---
id: 5fd9a02a5c9202a98b2f2ae1
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 针对对象属性的增删改操作
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
针对对象属性的增删改操作。

前面文章中我们介绍了通过点操作符或中括号操作符访问对象属性，你也可以使用点操作符或中括号操作符来更新对象的属性。

以前面介绍的 dog 对象为例：

var dog = {
  "name": "小花",
  "legs": 4,
  "tails": 1,
  "color": "black"
};

让我们更改它的名称为 "秋刀鱼"，这有两种方式来更新对象的 name 属性： 
dog.name = "秋刀鱼"; 
或 
dog["name"] = "秋刀鱼"; 
现在，dog.name 的值就不再是 "小花"，而是 "秋刀鱼"。可以通过控制台方式输出修改后的名称，确认修改后的名称是否与修改名称一致。

你也可以像更改属性一样给对象添加属性。

看看我们是如何给 dog 添加主人"owner" 属性：

dog.owner = "阿秋“;

或者

dog["owner"] = "阿秋";

现在当我们访问 dog.owner 时会得到 dog 对象的 owner 值为 "阿秋"。

我们同样可以删除对象的属性，例如下面代码会删除新增加的 owner 属性：

delete dog.owner;

在控制台执行完整代码如下：

var dog = {
  "name": "小花",
  "legs": 4,
  "tails": 1,
  "color": "black"
};

dog.name = "秋刀鱼"; 
console.log( dog.name  ); // => 秋刀鱼

dog.owner = "阿秋";
console.log( dog.owner  ); // => 阿秋

delete dog.owner; // => true


</section>

## Instructions
<section id='instructions'>

</section>

## Tests
<section id='tests'>

</section>

## Challenge Seed
<section id='challengeSeed'>

<div id='js-seed'>

```js

```

</div>



</section>

## Solution
<section id='solution'>


</section>
