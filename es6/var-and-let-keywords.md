---
id: 5fec2f61c56d78c86b9cc777
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: var 和 let 关键字区别及作用域
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
var 和 let 关键字区别及作用域。

我们在使用 ES6 编程的过程中，经常会使用到 var 和 let 关键字，两个关键字都可以声明变量，但是很多人不知道两者之前的区别，下面我们来详细说明下两个关键字。

使用 var 关键字来声明变量，会出现重复声明导致变量被覆盖却不会报错的问题：

var name = '于悄';
var name = '赵一';
console.log(name); // => 赵一

在上面的代码中，name 的初始值为'于悄'，然后又被覆盖成了'赵一'。

在小型的应用中，您可能不会遇到这样的问题，但是当您的代码规模变得特别庞大的时候，就可能会在不经意间覆盖了之前定义的变量。 这样的行为不会报错，导致了 debug 的产生，排查这种问题非常困难。

在 ES6 中引入了新的关键字 let 来解决 var 关键字带来的潜在问题。 如果在上面的代码中，使用了 let 关键字来代替 var 关键字，结果只会是一个---报错。

let name = '于悄';
let name = '赵一'; // => Uncaught SyntaxError: Identifier 'name' has already been declared

您可以在浏览器的控制台里看见上面的错误。 与 var 不同的是，当使用 let 的时候，同一名字的变量只能被声明一次。 

注意："use strict" 语句代表开启了严格模式，用于检测常见的代码错误以及"不安全"的行为，

例如：

"use strict";
x = 3.14; // => Uncaught ReferenceError: x is not defined


当您使用 var 关键字来声明一个变量的时候，这个变量会被声明成全局变量，或是函数内的局部变量。

let 关键字的作用类似，但会有一些额外的特性。如果在代码块、语句或表达式中使用 let 关键字声明变量，这个变量的作用域就被限制在当前的代码块、语句或表达式之中。

示例如下所示：

var numArray = [];
for (var i = 2; i < 6; i++) {
  numArray.push(i);
}

console.log(numArray); // => [2, 3, 4, 5]

console.log(i); // => 6


当使用 var 关键字的时候，i 会被声明成全局变量。当 i++ 执行的时候，它会改变全局变量的值。这段代码可以看做下面这样:

var numArray = [];
var i;
for (i = 2; i < 6; i++) {
  numArray.push(i);
}
console.log(numArray); // => [2, 3, 4, 5]
console.log(i); // => 6

如果在 for 循环中创建了使用 i 变量的函数，那么在后续调用函数的时候，上面提到的这种行为就会出现问题。这是因为函数存储的值会因为全局变量 i 的变化而不断的改变。

var numFun;
for (var i = 0; i < 3; i++) {
  if (i === 2) {
    numFun = function() {
      return i;
    };
  }
}
console.log(numFun()); // => 3

可以看到，numFun() 打印了 3 而不是 2。这是因为 i 发生了改变，并且函数 numFun() 返回的是全局变量 i 的值，而不是 for 循环中创建函数时 i 的值。let 关键字就不会有这种现象，调整为 let 关键字声明变量的代码如下所示：

'use strict';
let numFun2;
for (let i = 0; i < 3; i++) {
  if (i === 2) {
    numFun2 = function() {
      return i;
    };
  }
}
console.log(numFun2()); // => 2
console.log(i); // => ReferenceError: i is not defined

在控制台执行以上代码，最后在控制台会显示 ReferenceError: i is not defined， 提示变量 i 未定义。 i 在全局作用域中没有声明，所以它没有被定义，它的声明只会发生在 for 循环内。在循环执行的时候，let 关键字创建了三个不同的 i 变量，他们的值分别为 0、1 和 2，所以 numFun2() 返回了正确的值。


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
