---
id: 5fbb4ab3d7a713c76a7f3734
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:  转义字符串中的引号及常用转义序列使用
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
转义字符串中的引号及常用转义序列使用。

在 JavaScript 中，字符串必须使用单引号或者双引号来起始或者结束。如果想在字符里面包含 " 或者 ' 时该怎么办呢? 在 JavaScript 中，可以通过在引号前面使用反斜杠（\）来转义引号的方式实现。

var strMsg = "孙飞说, \"赵杰正在学习 JavaScript 语言\".";
console.log(strMsg); // ==> 孙飞说, "赵杰正在学习 JavaScript 语言".


有了转义符号，JavaScript 就知道这个单引号或双引号并不是字符串的结尾，而是字符串内的字符。所以，上面的字符串打印到控制台的结果为：

孙飞说, "赵杰正在学习 JavaScript 语言".

引号不是字符串中唯一可以被转义的字符。使用转义字符有两个原因：首先是可以让你使用无法输入的字符，例如退格。其次是可以让你在一个字符串中表示多个引号，而不会出错。下表为经常使用的转义序列：

代码		输出
\'		单引号
\"		双引号
\\		反斜杠
\n		换行符
\r		回车符
\t		制表符
\b		退格
\f		换页符

注意：必须对反斜杠本身进行转义才能显示为反斜杠。

使用转义序列定义一个变量如下所示：

var strMsg = "第一行 \n \\ 第二行 \n 第三行";
console.log(strMsg); 

代码执行后，会在控制台输出如下所示字符串：

第一行 
 \ 第二行 
 第三行


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
