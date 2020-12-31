---
id: 5fec2f61c56d78c86b9cc777
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: const 关键字用法详解
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
const 关键字用法详解。

在 ES6 中， let 关键字并不是唯一的新的声明变量的方式。在 ES6 里面，您还可以使用 const 关键字来声明变量。

const 拥有 let 的所有优点，所不同的是，通过 const 声明的变量是只读的。这意味着通过 const 声明的变量只能被赋值一次，而不能被再次赋值。


"use strict";
const USER_Name = "赵一";
USER_Name = "李翔"; // => Uncaught TypeError: Assignment to constant variable


在控制台执行以上代码，在控制台输出可以看见以上错误信息。尝试给通过 const 声明的变量再次赋值会报错。在日常的编码过程中，您应该使用 const 关键字来对所有不打算再次赋值的变量进行声明。这有助于避免给一个常量进行额外的再次赋值。一个最佳实践是对所有常量的命名采用全大写字母，并在单词之间使用下划线进行分隔。

注意： 一般开发者会以大写做为常量标识符，小写字母或者驼峰命名做为变量（对象或数组）标识符。接下来的文章里会涉及到小写变量标识符的数组。

在现代的 JavaScript 语言里，const 声明除了上面的用法外，还有很多其他用法。

一些开发者倾向默认使用 const 来声明所有变量，但如果它们打算在后续的代码中修改某个值，那在声明的时候就会用 let 关键字。

然而，在编程过程中，需要注意对象（包括数组和函数）在使用 const 声明的时候依然是可变的。使用 const 来声明只会保证它的标识不会被重新赋值。

"use strict";
const numArr = [5, 6, 7];
numArr = [1, 2, 3]; // => Assignment to constant variable
numArr[2] = 38; // 像使用 var 或 let 声明数组一样
console.log(numArr); // => [5, 6, 38]

从以上代码看出，可以改变[5, 6, 7]自身，所以 numArr 变量指向了改变后的数组 [5, 6, 38]。和所有数组一样，数组 numArr  中的数组元素是可以被改变的，但是因为使用了 const 关键字，不能使用赋值操作符将变量标识 numArr 指向另外一个数组。



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
