---
id: 606af4f0311cf78224358f51
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 了解对象原型链
---

## Description
<section id='description'>
![](http://www.icoderoad.com/p/images/data.png)

欢迎关注路条编程网站，本专题将教您如何操作数组，以及如何访问和复制数组中的信息。它还将教您如何操作和访问 JavaScript 对象中的数据，同时使用点和括号表示法。

了解对象原型链

JavaScript 中所有的对象（除了少数例外）都有自己的原型。而且，对象的原型本身也是一个对象。我们在介绍具体示例之前，先介绍下 typeof 操作符、isPrototypeOf() 方法和 hasOwnProperty() 方法的用法。

typeof 操作符返回一个字符串，表示未经计算的操作数的类型。

语法：

typeof 运算符后接操作数：

typeof operand

typeof(operand)

参数：

operand 一个表示对象或原始值的表达式，其类型将被返回。

isPrototypeOf() 方法用于测试一个对象是否存在于另一个对象的原型链上。

isPrototypeOf() 与 instanceof 运算符不同。在表达式 "object instanceof AFunction"中，object 的原型链是针对 AFunction.prototype 进行检查的，而不是针对 AFunction 本身。

语法：

prototypeObj.isPrototypeOf(object)

参数：

object 在该对象的原型链上搜寻

返回值：

Boolean，表示调用对象是否在另一个对象的原型链上。

hasOwnProperty() 方法会返回一个布尔值，指示对象自身属性中是否具有指定的属性（也就是，是否有指定的键）。

语法：

obj.hasOwnProperty(prop)

参数：

prop 要检测的属性的 String 字符串形式表示的名称，或者 Symbol。

返回值：

用来判断某个对象是否含有指定的属性的布尔值 Boolean。


function Site(name) {
  this.name = name;
}

console.log( typeof Site.prototype ); 
// => object

正因为原型是一个对象，所以原型对象也有它自己的原型！这样看来的话，Site.prototype 的原型就是 

Object.prototype：

console.log( Object.prototype.isPrototypeOf(Site.prototype) );
//=> true

这有什么作用呢？可能大家还记得我们在前篇文章中学到的 hasOwnProperty 方法：

let site = new Site("路条编程");
console.log( site.hasOwnProperty("name") ); 
// => true

hasOwnProperty 是定义在 Object.prototype 上的一个方法，尽管在Site.prototype 和  site 上并没有定义该方法，但是我们依然可以在这两个对象上访问到。这就是一个原型链。 

在这个原型链中，Site 构造函数是父级，site 是子级。Object 则是 Site 构造函数和 site 实例共同的父级。 Object 是 JavaScript 中所有对象的父级，也就是原型链的最顶层。因此，所有对象都可以访问 hasOwnProperty 方法。

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
