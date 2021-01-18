---
id: 5ffc11fc71bf0ff7cc3a83ab
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 class 语法定义构造函数
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用 class 语法定义构造函数。

ES6 提供了一个新的创建对象的语法，使用关键字 class。实际上，类 class 是“特殊的函数”，就像您能够定义的函数表达式和函数声明一样，类语法有两个组成部分：类表达式和类声明。

类表达式
类表达式是定义类的另一种方法。类表达式可以命名或不命名。命名类表达式的名称是该类体的局部名称。

类声明
定义类的一种方法是使用类声明。要声明一个类，可以使用带有 class 关键字的类名。

注意：class 只是一个语法，它并不像 Java、Python 或者 Ruby 这一类的语言一样，严格履行了面向对象的开发规范。

在 ES5 里面，我们通常会定义一个构造函数，然后使用 new 关键字来实例化一个对象：

var Site = function (name) {
  this.name = name;
}
var site = new Site('路条编程');

class 的语法只是简单地替换了构造函数的写法：

class Site {
  constructor(name) {
    this.name = name;
  }
}

const site = new Site('路条编程');

应该注意 class 关键字声明了一个函数，里面添加了一个构造器（constructor）。当调用 new 来创建一个新对象时构造器会被调用。

注意：首字母大写驼峰命名法是 ES6 class 名的惯例，就像上面的 Site。
构造函数是一个特殊的函数，在用 class 创建时来创建和初始化对象。在 JavaScript 算法和数据结构专题的面向对象部分我们会更深入介绍。

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
