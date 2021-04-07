---
id: 6067aa890396cc9086a97c4b
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 isPrototypeOf 方法来验证对象实例和原型的关系 
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

使用 isPrototypeOf 方法来验证对象实例和原型的关系

就像人从父母那里继承基因一样，对象也可直接从创建它的构造函数那里继承其原型。在介绍具体的实现代码之前，我们先介绍下 isPrototypeOf() 方法。

isPrototypeOf() 方法用于测试一个对象是否存在于另一个对象的原型链上。

isPrototypeOf() 与 instanceof 运算符不同。在表达式 "object instanceof AFunction"中，object 的原型链是针对 AFunction.prototype 进行检查的，而不是针对 AFunction 本身。

语法：

prototypeObj.isPrototypeOf(object)

参数：

object 在该对象的原型链上搜寻

返回值：

Boolean，表示调用对象是否在另一个对象的原型链上。

报错：

TypeError 如果 prototypeObj 为 undefined 或 null，会抛出 TypeError。


请看下面的例子：Bird构造函数创建了一个duck对象：

function Site(name) {
  this.name = name;
}

let site = new Site("路条编程");

site 从 Site 构造函数那里继承了它的原型，我们可以使用 isPrototypeOf 方法来验证他们之间的关系：

Site.prototype.isPrototypeOf( site );
// => true


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
