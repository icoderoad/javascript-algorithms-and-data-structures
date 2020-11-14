---
id: 56533eb9ac21ba0edf2244a8
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用赋值运算符存储值
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
使用赋值运算符存储值。

JavaScript 语言中的赋值运算可以分为简单和复合两种赋值运算，前者是将赋值运算符 = 右边表达式的值保存到左边的变量中，而后者是混合了其他的操作（例如算术运算符操作）和赋值操作相结合。

简单赋值运算符

最简单的赋值运算符应该就是等号 = ，把一个值赋给一个变量，例如我们学变量的使用，声明一个变量并给变量赋值可以写为 var a = 8 ，这就表示给变量 a 赋值为 8。

语法格式：

变量 = 数据

赋值运算符左边只能是变量，多个赋值运算符可以组成赋值表达式，它具有右结合性。如果赋值运算符的左侧也为一个数值则会报错：

console.log(7 = 6);  // SyntaxError: Invalid left-hand side in assignment

报错信息提示我们赋值中的左侧无效。

示例：

例如使用赋值运算符 = 给变量赋值：

var num1 = 98;
var num2 = num1;
console.log(num2);  // 输出：85

首先我们将等号右边的 Number 类型的值 85 赋值给左边的变量 num1，然后将等号右边的变量 num1 中存储的值，赋值给左边的变量 num2，最后输出 num2 的值也为 98。

记住遵循一个原则：从右往左计算。

复合赋值运算符

加赋值运算符是复合赋值运算符中的一种。加赋值运算符为 += ，用于把一个右值与一个变量相加，然后把相加的结果赋给该变量。两个操作数的类型决定了加赋值运算符的行为。算术相加或字符串连接都有可能。

+= 其实就是一个简写运算符的方式，例如 x += y 就是 x = x + y 的简写，这中方式在循环中经常会用到。

示例如下所示：

var x = 18;
x += 7;
console.log(x);  // 输出：25

执行这段代码，最后输出结果为 25。其中 x += 7 就相当于 x = x + 7 。

如果加赋值的是一个字符串类型的值，则返回的结果也为一个字符串值：

var a = 8;
a += '10';
console.log(a);  // 输出：810

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
