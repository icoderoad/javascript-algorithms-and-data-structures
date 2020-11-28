---
id: 5fc1985f5a8e70cb9f26738d
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:	数组描述及创建方式
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
数组描述及创建方式。

在程序语言中数组的重要性不言而喻，JavaScript 语言中数组也是最常使用的对象之一，数组是值的有序集合。由于弱类型的原因，JavaScript 语言中数组十分灵活、强大，不像是 Java 语言等强类型高级语言数组只能存放同一类型或其子类型元素，JavaScript 语言在同一个数组中可以存放多种类型的元素，而且是长度也是可以动态调整的，可以随着数据增加或减少自动对数组长度做更改。

在 JavaScript 语言中, 常使用构造函数和字面量两种方法创建数组。

构造函数

1.无参构造函数，创建一个开发语言的空数组

var devLangs = new Array();

2.一个数字参数构造函数，指定一个数组长度为 8，创建一个有 8 个元素的空数组，由于数组长度可以动态调整，设置数组元素个数作用不大。

var devLangs =new Array(8);

3.带有初始化数据的构造函数，创建数组 tmpArr 并使用数字、字符串及日期参数初始化数据

var tmpArr = new Array(4,'hello',new Date());

字面量

1.使用方括号，创建空数组，等同于调用无参构造函数

var devLangs=[];

2.使用中括号，并传入初始化数据，等同于调用调用带有初始化数据的构造函数

var devLangs=['JavaScript', 'html', 'css'];
console.log(devLangs); // ==> ["JavaScript", "html", "css"]

你也可以在数组中包含其他数组，例如：[["张三", 23], ["李四", 45]]。这被称为一个多维数组。

var userArr = [["张三", 23], ["李四", 45]];
console.log(userArr[0]); // ==> ["张三", 23] 将用户数组中第一个用户信息输出至控制台
console.log(userArr[1]); // ==> ["李四", 45] 将用户数组中第二个用户信息输出至控制台

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
