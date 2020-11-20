---
id: 56533eb9ac21ba0edf2244ac
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: JavaScript 中小数计算
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
JavaScript 中小数计算。

JavaScript 里的数字是采用 IEEE 754 标准的 64 位双精度浮点数。该规范定义了浮点数的格式，对于 64 位的浮点数在内存中的表示，最高的 1 位是符号位，接着的 11 位是指数，剩下的 52 位为有效数字，具体：

第 0  位：符号位， s 表示 ，0 表示正数，1 表示负数；
第 1  位到第 11 位：储存指数部分， e 表示 ；
第 12 位到第 63 位：储存小数部分（即有效数字），f 表示，

所有数字都是以 64 位浮点数形式储存，这样的存储结构优点是可以统一处理整数和小数，节省存储空间。 即便整数也是如此，所以我们在打印 1.00 这样的浮点数的结果是 1 而非 1.00 。

我们也可以把小数存储到变量中，小数也被称作浮点数 。

不是所有的实数都可以用浮点数来表示。因为可能存在四舍五入的错误，详情查看 https://en.wikipedia.org/wiki/Floating-point_arithmetic#Accuracy_problems , 此页面为英文页面，如果英语不好的话，可以使用百度翻译下相关内容。

以下代码为创建一个变量 myDecimal 并给它赋值一个浮点数。(例如 6.89 )。

var ourDecimal = 6.89;

在 JavaScript 中，您也可以像整数一样使用小数进行计算。

以下代码为把两个小数相乘，并得到它们乘积。

var val = 2.0 * 2.8;
console.log(val); // ==> 5.6

以下代码实现两个小数的除法运算，并得到它们的商：

var num = 4.4 / 2 ;
console.log(num); // ==> 2.2

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
