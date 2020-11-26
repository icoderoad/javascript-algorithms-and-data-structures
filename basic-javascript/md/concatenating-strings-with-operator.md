---
id: 5fbb4ab3d7a713c76a7f3734
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:  使用 + 或 += 运算符拼接字符串
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用 + 或 += 运算符拼接字符串。

在 JavaScript 中，当对一个 String 类型的值使用 + 操作符的时候，它被称作拼接操作符。可以通过拼接其他字符串来创建一个新的字符串。为了实现字符串的拼接，在 JavaScript 语言中， 常用两种方式实现字符串拼接。下面将通过代码实例详细介绍一下 JavaScript 如何实现字符串拼接操作。

方式一：使用加号（+）拼接

加号不但可以实现算数运算，也可以实现字符串拼接操作。

代码实例如下：

var webName="路条编程";

var address="北京市朝阳区";

var str= webName + "位于" + address + "!";

console.log(str); // ==> 路条编程位于北京市朝阳区!

注意：拼接操作不会在两个字符串之间添加空格，所以想加上空格的话，需要自己在字符串里面添加。

方式二：使用 += 复合运算符拼接

我们还可以使用 += 复合运算符来拼接字符串到现有字符串的结尾。对于那些被分割成几段的长的字符串来说，这一操作是非常有用的。还拿上面的字符串为例，拼接方式换成 += 方式，代码如下所示：

var webName="路条编程";

var address="北京市朝阳区";

var str = webName;
	str += "位于";
	str += address;
	str += "！";

console.log(str); // ==> 路条编程位于北京市朝阳区!

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
