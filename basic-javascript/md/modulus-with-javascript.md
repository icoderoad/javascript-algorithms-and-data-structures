---
id: 5fb769305c097284012e7677
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: JavaScript 取模运算
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
JavaScript 取模运算。

JavaScript 取模运算是一个表达式的值除以另一个表达式的值，并返回余数。

取模在 JavaScript 语言里就是取余数的意思。

a % b  //是求余数;

a / b  //是求商;

Math.abs(x)   //是求x的绝对值;

12 除以 5 = 2，余数是 2，即 5 * 2 + 2 = 12，所以 12 % 5 = 2

7 除以 3 = 2，余数是 1，即 3 * 2 + 1 = 7，所以 7 % 3 = 1 


在数学中，判断一个数是奇数还是偶数，只需要判断这个数除以 2 得到的余数是 0 还是 1。

17 % 2 = 1（ 17 是奇数 ）
48 % 2 = 0（ 48 是偶数 ）

注意：在这里要提醒大家要十分注意当前环境下'%'运算符的具体意义，因为在有负数存在的情况下，两者的结果是不一样的。

求模：

模等于 y - n * x ，n 是 y / x 后的商（要向下取整），算出模的值符号与 x 相同

7 / 3 的模  ， n = 7 / 3 为 2.3333，向下取整为 2，所以 n 等于 2

所以 7/3 的模是 7 - 2 * 3 = 1

var mod = 7%3;
console.log(mod); // ==> 1
 
7 / (-3) 的模，n = 7 / (-3) 为 -2.3333，向下取整为 -3，所以 n 等于 -3

所以 7 / (-3) 的模是 7 - （-3）*（-3）= -2


求余：

余数等于 y - n * x ，n 是 y/x 后的商（要向 0 取整），算出余数的值符号与 y 相同

7 / 3 的余数  ， n = 7 / 3 为 2.3333，向 0 取整为 2，所以 n 等于 2

所以 7 / 3 的余数是 7 - 2 * 3 = 1

 
7 / (-3) 的余数，n = 7 / (-3)为 -2.3333，向 0 取整为 -2，所以 n 等于 -2

所以 7 / (-3) 的余数是 7 - （-3）*（-2）= 1

求余和求模区别如下所示：

在计算 n 值的时候，求模（向下取整），取余（向 0 取整）
在计算 n 的符号的时候：求模（模的值与x的符号一样），取余（模的值与 y 的符号一样）


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
