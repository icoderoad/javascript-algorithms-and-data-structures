---
id: 5fc0a4afc7279e65873f7a31
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:	使用方括号获取字符串
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用方括号获取字符串。

前面的文章中我们介绍了通过方括号获取字符串的第一个和最后一个字符，也可以使用方括号来获取一个字符串中的其他位置的字符。

注意：JavaScript 语言是从 0 开始计数，所以获取第一个字符实际上是获取索引位置为 0 的字符。如果想要获取字符串的最后一个字符，可以用字符串的长度减 1 的索引值 ,例如获取网站名称中最后一个字符可以通过 siteName[siteName.length - 1] 实现。

让我们使用方括号，把 strSite 变量的第三个字符赋值给变量 str3Site ，代码如下所示：

var strSite = "路条编程";
var str3Site = strSite[2]; 
console.log( str3Site ); // ==> 编


我们既可以获取字符串的最后一个字符，也可以用获取字符串的倒数第 N 个字符。

例如，你可以这样 subject[subject.length - 3] 操作来获得 var subject = "本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等" 字符串中的倒数第三个字符。

var subject = "本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等";
var subStr = subject[subject.length - 3];
console.log(subStr); // ==> 语


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
