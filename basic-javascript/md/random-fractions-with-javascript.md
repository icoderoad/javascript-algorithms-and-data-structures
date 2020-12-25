---
id: 5fe5a44dfe8568f33b0061d9
challengeType: 1
videoUrl: ''
forumTopicId: -1
title:  JavaScript 语言中随机数的使用
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
JavaScript 语言中随机数的使用。

随机数非常适合用来创建随机行为。

为了生成随机数，JavaScript 语言中通过 Math.random() 函数实现。Math.random() 函数返回一个浮点数,  伪随机数在范围从 0 到小于 1，也就是说，从 0（包括 0 ）往上，但是不包括 1（排除 1 ），然后您可以缩放到所需的范围。实现将初始种子选择到随机数生成算法，它不能被用户选择或重置。

由于 Math.random() 函数生成的都是小数，但随机数更有用的地方在于生成随机整数。为了实现生成随机整数，我们需要如何实现呢？可以通过 Math.random() 生成一个随机小数。把这个随机小数乘以 10 的整数倍，用 Math.floor() 向下取整获得它最近的整数。

由于 Math.random() 函数永远不会返回 1 。我们又使用 Math.floor() 向下取整，所以最终我们获得的结果不可能有 10 的整数倍整数。这确保了我们获得了一个在 0 到 10 的整数倍之间的整数。

我们以生成一个 0 到 9 之间的随机整数为例，代码如下所示：

var num =  Math.floor(Math.random() * 10);
console.log( num ); // => 2

以上代码我们先调用 Math.random() 函数生成一个随机小数，把它的结果乘以 10，然后把上一步的结果传给 Math.floor() 函数，最终通过向下取整获得最近的整数赋值给变量 num , 然后在控制台将随机数输出。我们测试时生成的随机数为2，大家测试时每次执行都会生成 0 到 9 之间不同的整数。

上面我们通过算法实现的是生成 0 到某个数之间的随机数，如果我们要生成在两个指定的数之间的随机数，我们如何操作呢？我们可以通过定义一个最小值和一个最大值的方式实现。

下面是我们将要使用的方法，需要定义一个指定区间的最大值 max 和最小值 min，然后通过 Math.random 和 Math.floor 函数通过下面的公式生成随机数：

var max =100;
var min = 80;
var num = Math.floor(Math.random() * (max - min + 1)) + min
console.log(num); // => 87

以上代码我们生成了一个 80 到 100 之间的随机数，然后在控制台输出。大家可以在控制台执行下上面代码，每次都会生成一个 80 到 100 之间的随机数。 

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
