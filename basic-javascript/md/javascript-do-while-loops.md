---
id: 5fe1917337c23adfb0d59cf7
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: do...while 循环语句用法详解
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 JavaScript 基本语法、注释、变量声名、各种运算符、字符串、数组及条件语句等。通过学习 JavaScript 算法及数据结构这一系列文章，你将会逐步掌握 JavaScript 基础相关的知识。
	
do...while 循环语句用法详解。

今天我们介绍 JavaScript 语言中的第三种循环类型 do...while 循环。

do...while 语句一直重复直到指定的条件求值得到假值（false）。

语法示例如下所示：

do
  语句块
while (执行条件);

语句块 在检查条件之前会执行一次。要执行多条语句（语句块），要使用块语句（{ ... }）包括起来。 如果 执行条件 为真（true），语句块 将再次执行。 在每个执行的结尾会进行条件的检查。当 执行条件 为假（false），执行会停止并且把控制权交回给 do...while 后面的语句。

do-while 与 while 循环的不同之处在于: 它先执行循环中的语句,然后再判断表达式是否为真, 如果为真则继续循环；如果为假, 则终止循环。因此, do-while 循环至少要执行一次循环语句。

我们来看一个例子。

var arr = [];
var i = 0;
do {
  arr.push(i);
  i++;
} while (i < 3);
console.log(arr); // => [0, 1, 2]

这看起来和其他循环语句差不多，返回的结果是[0, 1, 2]，do...while 与其他循环不同点在于，初始条件为假时的表现，让我们通过实际的例子来看看。 这是一个普通的 while 循环，只要 i < 3，它就会在循环中运行代码。

var arr = []; 
var i = 3;
while (i < 3) {
  arr.push(i);
  i++;
}
console.log(arr); // => []

注意，我们首先将 i 的值初始化为 3。执行下一行时，注意到 i 不小于 3 ，循环内的代码将不会执行。所以 arr 最终没有添加任何内容，因此示例中的所有代码执行完时，arr 仍然是[]。 现在，看一下 do...while 循环。

var arr = []; 
var i = 3;
do {
  arr.push(i);
  i++;
} while (i < 3);
console.log(i); // => 4
console.log(arr); // [3]

在这里，和使用 while 循环时一样，我们将 i 的值初始化为 3。执行下一行时，没有检查 i 的值，直接执行花括号内的代码。数组会添加一个元素，并在进行条件检查之前递增 i。然后，在条件检查时因为 i 等于 4 不符合条件 i < 3，所以退出循环。最终 arr 的值是 [3]。 本质上，do...while 循环确保循环内的代码至少运行一次。 让我们通过 do...while 循环将值添加到数组中。

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
