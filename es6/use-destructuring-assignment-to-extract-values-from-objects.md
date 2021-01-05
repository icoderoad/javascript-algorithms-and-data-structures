---
id: 5ff41e8a6021a6526658f7f7
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用解构赋值来获取对象的值
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用解构赋值来获取对象的值。

解构赋值 是 ES6 引入的新语法，用来从数组和对象中提取值，并优雅的对变量进行赋值。

有如下 ES5 代码：

const site = { name: '路条编程', domain: 'www.icoderoad.com' };

const name = site.name; 
console.log(name); // => 路条编程
const domain = site.domain; 
console.log(domain); // => www.icoderoad.com

下面是使用 ES6 解构赋值的等价语句：
const site = { name: '路条编程', domain: 'www.icoderoad.com' };
const { name, domain } = site;
console.log(name); // => 路条编程
console.log(domain); // => www.icoderoad.com


在这里，name 和 domain 被自动创建并赋予 site 对象相应属性的值。一目了然。

上面的代码介绍的是解构对象的基本赋值，下面我们来介绍下无声明赋值。

一个变量可以独立于其声明进行解构赋值。

var name, domain;

({name, domain} = {name: '路条编程', domain: 'www.icoderoad.com'});
console.log(name, domain); // => 路条编程 www.icoderoad.com

注意：赋值语句周围的圆括号 ( ... ) 在使用对象字面量无声明解构赋值时是必须的。

{name, domain} = {name: '路条编程', domain: 'www.icoderoad.com'} 不是有效的独立语法，因为左边的 {name, domain} 被认为是一个块而不是对象字面量。

然而，({name, domain} = {name: '路条编程', domain: 'www.icoderoad.com'}) 是有效的，正如 var {name, domain} = {name: '路条编程', domain: 'www.icoderoad.com'} 一样，也是有效的。

您的 ( ... ) 表达式之前需要有一个分号，否则它可能会被当成上一行中的函数执行。


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
