---
id: 5fbf56f701f1fdef9e85f8c8
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:  理解 JavaScript 语言中字符串的不变性
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
理解 JavaScript 语言中字符串的不变性。

不变性是函数式编程中的核心原则，在很多面向对象程序中也都有所体现。本文将详细地说明什么是不变性、如何在 JavaScript 语言中使用这个概念以及为什么它是有用的。

什么是不变性？

可变性的文本定义是“易于改变或变化的”。在编程中，我们使用这个词来表示允状态随时间而变化的对象。一个不可改变的值的定义是完全相反的——在被创建之后，它永远不会改变。

在 JavaScript 语言中，字符串的值是不可变的，这意味着一旦字符串被创建就不能被改变。

例如，下面的代码：

var strSite = "路条编程";
strSite[0] = "头";
console.log( strSite ); // ==> 路条编程

是不会把变量 strSite 的值改变成 "头条编程" 的，因为变量 strSite 是不可变的。

注意，这并不意味着 strSite 永远不能被改变，只是字符串字面量 string literal 的各个字符不能被改变。

改变 strSite 中的唯一方法是重新给它赋一个值，例如：

var strSite = "路条编程";
strSite = "头条编程";
console.log( strSite ); // ==> 头条编程


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
