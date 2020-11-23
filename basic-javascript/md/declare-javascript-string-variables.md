---
id: 5fba220104e028487a94d5cc
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 字符串变量声明及使用
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
字符串变量声明及使用。

在前面的文章中我们已经介绍过变量的声名及命名规则，现在我们介绍下字符串的声明。在 JavaScript 语言中，使用变量步骤为 a.声明-->b.赋值-->3.调用。 如果要声明一个变量，通过使用 var 关键词先进行声明，然后赋值，最后使用变量。以下为声明及使用字符串的两种方式：

// 方式一  声明和赋值同时进行

var strHello = "您好，欢迎访问路条编程";
console.log( strHello ); // ==> 您好，欢迎访问路条编程

// 方式二 先声明后赋值
var strHello;
strHello = '您好，欢迎访问路条编程';
console.log( strHello ); // ==> 您好，欢迎访问路条编程


以上代码中， "您好，欢迎访问路条编程" 被称作字符串变量值。字符串是用单引号或双引号包裹起来的一连串的零个或多个字符。

上面示例声明的都是单行字符串，如果想声明多行字符串，应该如何操作呢。工作中，常用两种方式进行多行字符串声明。

// 方式一  字符串拼接方式
var strHello = "codeLife，" +
			   "您好！" + 
			   "欢迎访问路条编程网站!" ;
console.log( strHello ); // ==> codeLife，您好！欢迎访问路条编程网站!

通过字符串拼接的方式声明多行字符串变量，一定要注意非最后行字符串一定以 + 结束， 最后一行以 ; 结束，不然会报语法错误。


// 方式二 转义行方式
var strHello = "\
			codeLife，\
			您好！\
			欢迎访问路条编程网站!" ;
console.log( strHello ); // ==> codeLife，您好！欢迎访问路条编程网站!

需要注意的是,通过转义行方式声明字符串变量时，非结束行结束开始不用加 ", 结束行只需以 \ 结束，不用以 ” 结束。当输出字符串时，换行符是不会显示出来的。如果需要真实的换行,必须在反斜杠前面加上一个 \n。



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
