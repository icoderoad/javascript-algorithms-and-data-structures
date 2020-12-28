---
id: 5fe7172be23388b2fd56a671
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: JavaScript 语言中 parseInt 函数用法详解
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
JavaScript 语言中 parseInt 函数用法详解。

我们在日常编程过程中，经常会遇到不同数据类型转换的问题。用得比较多的是字符串转换为整型，还有一些常用的不同进制转换。如果要实现数字之间不同类型转换及进制转换，我们在 JavaScript 语言中可以通过 parseInt 函数实现。parseInt 函数将其第一个参数转换为一个字符串，对该字符串进行解析，然后返回一个整数或 NaN。

语法示例：

parseInt(string, radix);

参数说明：

string 要被解析的值。如果参数不是一个字符串，则将其转换为字符串(使用  ToString 抽象操作)。字符串开头的空白符将会被忽略。
radix  可选参数，从 2 到 36，表示字符串的基数。例如指定 16 表示被解析值是十六进制数。请注意，10 不是默认值！

返回值：

从给定的字符串中解析出的一个整数。或者 NaN，当 radix 小于 2 或大于 36 ，或第一个非空格字符不能转换为数字。

下面是一个字符串返回一个整数的示例：

var num = parseInt("008");
console.log(num); // => 8

上面的代码把字符串 "008" 转换成数字 8 并赋值给变量 num 并在控制台将变量 num 输出，最终控制台输出数字 8。 如果字符串参数的第一个字符是字符串类型的，结果将不会转换成数字，而是返回 NaN。

下面是一个基数的转换示例：

var num = parseInt("123", 5);
console.log( num ); // => 38

参数 5 表示字符串 "123" 使用 5 进制数值系统。此示例将字符串 "123" 按 5 进制进行整数转换，返回十进制数为 38。转换过程如下：
38 => 1*5^2 + 2*5^1 + 3*5^0 = 38 。将转换后结果赋值给变量 num ,在控制台将变量 num 输出，最终控制台显示 38。

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
