---
id: 5ff018cea2c36264f8c5b92f
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用箭头函数编写简洁的匿名函数
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用箭头函数编写简洁的匿名函数。

在 JavaScript 语言里，我们经常会遇到不需要给函数命名的情况，尤其是在需要将一个函数作为参数传给另外一个函数的时候。这时，我们会创建匿名函数。因为这些函数不会在其他地方复用，所以我们不需要给它们命名。

这种情况下，我们通常会使用以下语法：

const myFunc = function() {
  const myVar = "value";
  return myVar;
}

ES6 提供了其他写方式匿名函数的的语法。您可以使用箭头函数写匿名函数。箭头函数表达式的语法比函数表达式更简洁，并且没有自己的 this、arguments、super 或 new 和 target。箭头函数表达式更适用于那些本来需要匿名函数的地方，并且它不能用作构造函数。

基础语法：

(param1, param2, …, paramN) => { statements }
(param1, param2, …, paramN) => expression
//相当于：(param1, param2, …, paramN) =>{ return expression; }

// 当只有一个参数时，圆括号是可选的：
(singleParam) => { statements }
singleParam => { statements }

// 没有参数的函数应该写成一对圆括号。
() => { statements }

高级语法：

//加括号的函数体返回对象字面量表达式：
params => ({foo: bar})

//支持剩余参数和默认参数
(param1, param2, ...rest) => { statements }
(param1 = defaultValue1, param2, …, paramN = defaultValueN) => {
statements }


我们修改上面匿名函数的通常写法为箭头函数，代码如下所示：

const myFunc = () => {
  const myVar = "value";
  return myVar;
}

当不需要函数体，只返回一个值的时候，箭头函数允许省略 return 关键字和外面的大括号。这样就可以将一个简单的函数简化成一个单行语句。

const myFunc = () => "value";

这段代码仍然会返回 value 。

我们练习一个简单的例子，下面是一个通常写法的 getDate 函数：

var getDate = function() {
  "use strict";
  return new Date();
};

使用箭头函数的语法重写 getDate 函数，使其返回一个新的 Date() 。同时不要用 var 关键字来定义任何变量。

const getDate = ()=> new Date();
console.log( getDate() ); // => Sat Jan 02 2021 15:10:12 GMT+0800 (中国标准时间)

以上代码为通过箭头函数改写后的 getDate 函数，代码更简洁。

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
