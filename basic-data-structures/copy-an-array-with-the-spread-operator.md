---
id: 60349170045d7b7273f04523
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用扩展运算符复制数组
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用扩展运算符复制数组

前面文章介绍的 slice() 方法已经能让我们从一个数组中选择一些元素来复制到新数组中了，而 ES6 中又新引入了一个简洁且可读性强的语法展开运算符，它能让我们方便地复制数组中的所有元素。

展开语法(Spread syntax), 可以在函数调用/数组构造时, 将数组表达式或者 string 在语法层面展开，还可以在构造字面量对象时, 将对象表达式按 key-value 的方式展开。

语法：myFunction(...iterableObj);

没有展开语法的时候，只能组合使用 push, splice, concat 等方法，来将已有数组元素变成新数组的一部分。有了展开语法,  通过字面量方式, 构造新数组会变得更简单、更优雅：

var parts = ['菜鸟001', '欢迎'];
var welcomeMsg = ['您好', ...parts, '访问', '路条编程！']; 
console.log( welcomeMsg );
// => (5) ["您好", "菜鸟001", "欢迎", "访问", "路条编程！"]

和参数列表的展开类似,  ... 在构造字面量数组时, 可以在任意位置多次使用.

数组拷贝(copy)
var welcomeMsgs = ['您好','菜鸟001', '欢迎', '访问' ];
var siteMsg = [...welcomeMsgs]; // 与 slice() 方法效果相同
siteMsg.push('路条编程');
console.log( siteMsg );
// => (5) ["您好", "菜鸟001", "欢迎", "访问", "路条编程"]

console.log( welcomeMsgs );
// => (4) ["您好", "菜鸟001", "欢迎", "访问"]

以上代码可知，通过控制台的输出结果可知， siteMsg 此时变成 “ ["您好", "菜鸟001", "欢迎", "访问", "路条编程"] ”， welcomeMsgs 结果仍为 “ ["您好", "菜鸟001", "欢迎", "访问"] ”，没受影响。

连接多个数组
Array.concat 函数常用于将一个数组连接到另一个数组的后面。如果不使用展开语法, 代码可能是下面这样的:

var welcomeMsgs1 = ['您好','菜鸟001'];
var welcomeMsgs2 = ["欢迎", "访问", "路条编程"];

// 将 arr2 中所有元素附加到 arr1 后面并返回

var welcomeMsgs3 = welcomeMsgs1.concat(welcomeMsgs2);
console.log( welcomeMsgs3 );
// => (5) ["您好", "菜鸟001", "欢迎", "访问", "路条编程"]

使用展开语法:

var welcomeMsgs4 = ['您好','菜鸟001'];
var welcomeMsgs5 = ["欢迎", "访问", "路条编程"];
var welcomeMsgs6 = [...welcomeMsgs4, ...welcomeMsgs5];
console.log( welcomeMsgs6 );
// => (5) ["您好", "菜鸟001", "欢迎", "访问", "路条编程"]


在实践中，我们可以这样用展开运算符来复制一个数组：

let msgArr = ["您好", "菜鸟001", "欢迎", "访问", "路条编程"];
let msgArr2 = [...msgArr];
console.log( msgArr );
// => ["您好", "菜鸟001", "欢迎", "访问", "路条编程"]

console.log( msgArr2 );
// => ["您好", "菜鸟001", "欢迎", "访问", "路条编程"]

以上代码在控制台输出数组 msgArr 和 msgArr2,   msgArr2 输出结果为 ["您好", "菜鸟001", "欢迎", "访问", "路条编程"]， msgArr 和原来一致，没有变化。


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
