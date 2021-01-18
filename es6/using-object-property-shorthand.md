---
id: 5ff9739ad60b111d0178c314
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用简单字段编写简洁对象字面量声明
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用简单字段编写简洁对象字面量声明。

ES6 添加了一些很实用的功能，以便于更方便地定义对象。

请看以下代码示例：

const getMousePosition = (x, y) => ({
  x: x,
  y: y
});

getMousePosition 是一个常规函数，返回了拥有 2 个属性对象的简单函数。 ES6 提供了一个语法，消除了类似 x: x 这种冗余的写法。可以仅仅只写一次 x，解释器会自动将其转换成 x: x 。 下面是使用这种语法重写的同样的函数：

const getMousePosition = (x, y) => ({ x, y });

通过上面的学习，我们现在使用简单属性对象的语法来创建并返回一个 Site 对象。

const Site = (name, telphone, domain) => {
  "use strict";
  return {
    name,
    telphone,
    domain
  };
};

console.log(Site('路条编程', '010-12987654', 'www.icoderoad.com'));
// => {name: "路条编程", telphone: "010-12987654", domain: "www.icoderoad.com"}


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
