---
id: 5ffad726ca3ee568fa502c48
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 用 ES6 编写简洁的函数声明
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
用 ES6 编写简洁的函数声明。

在 ES5 中，当我们需要在对象中定义一个函数的时候，我们必须如下面这样使用 function 关键字来定义函数：

const site = {
  name: "路条编程",
  welcomeMsg: function() {
    return `您好，欢迎访问 ${this.name}。`;
  }
};

console.log( site.welcomeMsg() );
// => 您好，欢迎访问 路条编程。

在 ES6 语法对象中定义函数的时候，您可以完全删除 function 关键字和冒号。请看调整以后 ES6 例子：

const site = {
  name: "路条编程",
  welcomeMsg() {
    return `您好，欢迎访问 ${this.name}。`;
  }
};
console.log( site.welcomeMsg() );
// => 您好，欢迎访问 路条编程。

上面的站点名称是固定的 路条编程，我们再调整下这个对象，增加一个方法，可以设置站点的名称，然后再调用欢迎信息的方法。调整后的代码如下所示：

const site = {
  name: "路条编程",
  setName( name ) {
  	this.name = name;
  },

  welcomeMsg() {
    return `您好，欢迎访问 ${this.name}。`;
  }
};
site.setName('路条公众号');
console.log( site.welcomeMsg() );
// => 您好，欢迎访问 路条公众号。

上面的代码增加了 setName 方法，方法参数 name 传给对象属性 this.name, 设置为新的属性 name, 然后在控制台输出 welcomeMsg 方法内容。我们在控制台输出了新设置的 “路条公众号”。

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
