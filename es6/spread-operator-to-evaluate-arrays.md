---
id: 5ff2a8a311e71abe503c3f9d
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 spread 运算符展开数组项
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用 spread 运算符展开数组项。

ES6 允许我们使用 展开操作符 来展开数组，以及需要多个参数或元素的表达式。展开操作符, 可以在函数调用/数组构造时, 将数组表达式或者 string 在语法层面展开。还可以在构造字面量对象时, 将对象表达式按 key-value 的方式展开。

下面的 ES5 代码使用了 apply() 来计算数组的最大值：

var arr = [5, 88, 2, 69];
var maximus = Math.max.apply(null, arr); 
console.log(maximus); // => 88

我们必须使用 Math.max.apply(null,arr)，是因为直接调用 Math.max(arr) 会返回 NaN。Math.max() 函数需要传入的是一系列由逗号分隔的参数，而不是一个数组。 展开操作符可以提升代码的可读性，这对后续的代码维护是有积极作用的。

const arr = [6, 108, 3, 45];
const maximus = Math.max(...arr); 
console.log(maximus); // => 108

...arr 返回了一个“打开”的数组。或者说它 展开 了数组。 然而，展开操作符只能够在函数的参数中，或者数组之中使用。下面的代码将会报错：

const spreaded = ...arr; // Uncaught SyntaxError: Unexpected token '...'


下面我们练习一个数组赋值的示例：

const weekdays = ['周一', '周二', '周三', '周四', '周五', '周六', '周日'];
let arr2;
arr2 = [];  
arr2= [...weekdays];
console.log(arr2); // => ["周一", "周二", "周三", "周四", "周五", "周六", "周日"]

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
