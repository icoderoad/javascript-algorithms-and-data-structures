---
id: 5fca17ac570b63d795739011
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 函数返回值及返回值赋值
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
函数返回值及返回值赋值。

函数一般用 return 语句来返回值，但这不是必须的。在函数没有 return 语句的情况下，当你调用它时，该函数会执行内部代码，返回的值是 undefined 。

函数返回无返回值示例如下所示：

var sum = 0;
function addSum(num) {
  sum = sum + num;
}
console.log(addSum(3)); // => undefined
console.log(sum); // => 3

addSum 函数是一个没有 return 语句的函数。该函数将更改全局变量 sum ，函数的返回值为 undefined 。

如果你还记得我们在前端文章中使用赋值运算符存储值的的内容，赋值之前，先完成等号右边的操作。这意味着我们可把一个函数的返回值，赋值给一个变量。

假设我们调整 addSum 函数，将其修改为有返回值的函数，将相加后的结果赋值给变量 total ,那么，调整代码如下所示：

var sum = 0;
function addSum(num) {
  return sum = sum + num;
}

var total = addSum(12); // total = 12
total += addSum(18); // 12 + 30 => 42
console.log(total); // => 42

调用 addSum 函数,参数赋值 12，然后将返回值 return 一个 sum 变量 + 12 的数值 12，然后把它赋值给了 total 变量， 再次执行 total 加 addSum 函数的结果，然后将
total 变量在控制台输出为 42。

## Instructions
<section id='instructions'>

</section>

## Tests
<section id='tests'>
函数一般用return语句来返回值，但这不是必须的。在函数没有return语句的情况下，当你调用它时，该函数会执行内部代码，返回的值是undefined。

示例

var sum = 0;
function addSum(num) {
  sum = sum + num;
}
addSum(3); // sum will be modified but returned value is undefined
addSum是一个没有return语句的函数。该函数将更改全局变量sum，函数的返回值为undefined。



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
