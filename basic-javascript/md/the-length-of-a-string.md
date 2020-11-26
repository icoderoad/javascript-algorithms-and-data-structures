---
id: 5fbe0e4add9468b0fe624394
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:  获取字符串长度及获取字符串中指定位置字符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
取字符串长度及获取字符串中指定位置字符。

在 JavaScript 语言中，使用字符串的 length 属性可以获取字符串的长度。长度以字符为单位，该属性为只读属性。

我们拿上篇文章的示例字符串变量为例，如果想获取 str 变量的长度，并把它赋值给变量 strLength，并将字符串长度在控制台输出。 通过以下代码实现：

var webName="路条编程";

var address="北京市朝阳区";

var str = webName;
	str += "位于";
	str += address;
	str += "！";

var strLength = str.length;

console.log(strLength); // ==> 13


方括号表示法是一种在字符串中的特定位置获取字符的方法。

大多数现代编程语言，如 JavaScript 语言，不同于人类语言从 1 开始计数，JavaScript 语言是从 0 开始计数，这被称为基于零的索引。

例如, 想获取变量 str 中获 第一个字符为 "路"，使用方括号[]获取变量 str 中的第一个字符，并赋给变量 firstLetter, 并将结果在控制台输出，代码如下所示：


var firstLetter = str[0];
console.log(firstLetter); // ==> 路

注意：如果想在控制台可以正常输出，需要将第一二两部分代码同时在控制台执行。

如果想获取公司位置字符串的最后一个字符，我们如何实现呢？可以通过方括号[] 和字符串 length 属性实现。代码如下所示：

var lastLetter = str[ str.length -1];
console.log(lastLetter); // ==> !

注意：由于 JavaScript 语言的索引是从 0 开始的，如果想获取字符串最后一个字符，应该使用字符串长度 -1 得到最后字符串索引。

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
