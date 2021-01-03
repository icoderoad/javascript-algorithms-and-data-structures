---
id: 5ff108b5bcd4f956ac44cb7b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 函数默认参数与 rest 操作符
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
函数默认参数与 rest 操作符。

ES6 里允许给函数传入默认参数，来构建更加灵活的函数。前面文章中我们介绍了箭头函数，现在给大家介绍下带有默认参数的箭头函数。

请看以下代码：

const greeting = (name = "吴明") => "您好，" + name;

console.log(greeting("张峰")); // => 您好，张峰
console.log(greeting()); // => 您好，吴明


默认参数会在参数没有被指定（值为 undefined ）的时候起作用。在上面的例子中，参数 name 会在没有得到新的值的时候，使用默认值 "吴明"。还可以给多个参数赋予默认值。

请看下面的例子：
 
给函数 increment 加上默认参数，使得在 value 没有被赋值的时候，默认给 number 加 8。

const increment = (number=12, value=8) => number + value;
console.log(increment()); // => 20
console.log(increment(13, 9)); // => 22

上面的例子中，我们在箭头函数下面执行两个 increment 函数调用，第一行直接调用 increment 函数，没有给函数任何参数，参数 number、value 都使用默认值 12、8 ，调用后，在控制台输出 20。第二行传入两个参数分别为 13、9，函数调用后计算两个参数之和，在控制台输出 22。

ES6 推出了用于函数参数的 rest 操作符，帮助我们创建更加灵活的函数。

在 rest 操作符的帮助下，您可以创建有一个变量来接受多个参数的函数。这些参数被储存在一个可以在函数内部读取的数组中。

我们修改下上面的 increment 函数，调整后的代码如下所示：

const increment = (...values) =>{
  let sum = 0;

  for (var val of values) {
    sum += val;
  }

  return sum;
}

console.log(increment(13, 36, 18)); // => 67
console.log(increment(27, 42, 89)); // => 158

以上代码使用了 rest 操作符，可以通过 values 参数接收传入的多个参数值，然后通过 for 循环进行遍历求和，返回多个参数的和。

rest 操作符可以避免查看 args 数组的需求，并且允许我们在参数数组上使用 map()、fiter() 和 reduce()。

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
