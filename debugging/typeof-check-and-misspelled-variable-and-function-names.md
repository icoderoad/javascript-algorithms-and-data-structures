---
id: 60221f14eaf4f4648358bef1
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 type of 检查变量的类型和变量名和函数名检测
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/regex.png)

欢迎关注路条编程网站，本专题主要介绍 一些有用的工具来查找 bug，以及它们采取的一些常见形式。幸运的是，调试是一项可以学习的技能，只需要一点耐心和练习就可以掌握。

使用 type of 检查变量的类型和变量名和函数名检测

我们在平时调试程序时，可以使用 typeof 检查变量的数据结构或类型。在处理多种数据类型时，typeof 会对调试很有帮助。如果想计算两数之和，但实际传入了一个字符串参数，则结果可能是错误的。类型错误可能隐藏在计算或函数调用中。以 JavaScript 对象（JSON）的形式访问和使用外部数据时尤其要小心。

下面是使用 typeof 的一些示例：

console.log( typeof ""); 
// => string

console.log( typeof 0 ); 
// => number

console.log( typeof [] ); 
// => object
console.log(typeof {}); 
// => object

JavaScript 有六种原始（不可变）数据类型：Boolean, Null, Undefined, Number, String, 和 Symbol（ES6 新增）和一种可变的数据类型：Object。
注意，在 JavaScript 语言中，数组在本质上是一种对象

console.log() 和 typeof 方法是检查中间值和程序输出类型的两种主要方法。 现在我们了解一下 bug 出现的常见情形。一个语法级别的问题是打字太快带来的低级拼写错误。

变量或函数名的错写、漏写或大小写弄混都会让浏览器尝试查找并不存在的东西，并报出“引用错误”。JavaScript 语言中变量和函数名称区分大小写。

下面我们做个练习，代码示例如下所示：

let num1 = 29;
let Num2 = 12;
let total = num1 + num2;
console.log(`两数的和为: ${total}`);

在控制台执行以上代码，控制台应该输出 "两数的和为: 41"。代码执行后，控制台没有输出正确的结果，在控制输出如下错误信息：

Uncaught ReferenceError: num2 is not defined

由于 JavaScript 语言中变量名称是区分大小写的，我们在定义时变量名称为 Num2， 求和计算时将变量名写成了小写的 num2，所以会报以上错误，调整为大写变量名后，代码如下所示：

let num1 = 29;
let Num2 = 12;
let total = num1 + Num2;
console.log(`两数的和为: ${total}`);

再次在控制台执行以上代码，控制台输出 “两数的和为: 41”， 控制台输出结果与预期结果一致。

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
