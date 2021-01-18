---
id: 5ffd35436a96e7f50e534eb4
challengeType: 1
videoUrl: ''
forumTopicId: -1
title: 使用 getter 和 setter 来控制对象的访问
---

## Description
<section id='description'>
![](https://www.icoderoad.com/javascript/basic-javascript/images/jsdata.png)

欢迎关注路条编程网站，本专题主要介绍 ES6 新的语法、箭头函数、解构、类定义、模块、Promise 异步操作、生成器函数、let 和 const 关键字等。通过学习  ES6 这一系列文章，你将会逐步掌握  ES6 基础相关的知识。
	
使用 getter 和 setter 来控制对象的访问。

前面文章中，我们介绍了通过对象方法给对象属性赋值。现在我们介绍 getters 以及 setters 从对象中获取值或给对象的属性赋值。

Getter 函数的作用是可以让对象返回一个私有变量，而不需要直接去访问私有变量。

语法：
{get prop() { ... } }
{get [expression]() { ... } }

参数：
prop	要绑定到给定函数的属性名。
expression	从 ECMAScript 2015 开始，还可以使用一个计算属性名的表达式绑定到给定的函数。

有时需要允许访问返回动态计算值的属性，或者可能需要反映内部变量的状态，而不需要使用显式方法调用。在 JavaScript 中，可以使用 getter 来实现。

尽管可以结合使用 getter 和 setter 来创建一个伪属性，但是不可能同时将一个 getter 绑定到一个属性并且该属性实际上具有一个值。

使用get语法时应注意以下问题：

可以使用数值或字符串作为标识；
必须不带参数
它不能与另一个 get 或具有相同属性的数据条目同时出现在一个对象字面量中

Setter 函数的作用是可以基于传进的参数来修改对象中私有变量。这些修改可以是计算，或者是直接替换之前的值。

语法：
{set prop(val) { . . . }}
{set [expression](val) { . . . }}

参数：
prop
要绑定到给定函数的属性名。
val
用于保存尝试分配给prop的值的变量的一个别名。
表达式
从 ECMAScript 2015 开始，还可以使用一个计算属性名的表达式绑定到给定的函数。

在 javascript 中，如果试着改变一个属性的值，那么对应的 setter 将被执行。setter 经常和 getter 连用以创建一个伪属性。不可能在具有真实值的属性上同时拥有一个 setter 器。

使用 set 语法时请注意：

它的标识符可以是数字或字符串
它必须有一个明确的参数 
在对象字面量中，不能为一个已有真实值的变量使用 set ，也不能为一个属性设置多个 set。


class Site {

  constructor(name) {
    this._name = name;
  }
  // getter
  get name() {
    return this._name;
  }
  // setter
  set name(updatedName) {
    this._name = updatedName;
  }
}
const site = new Site('路条编程');
console.log(site.name);  // => 路条编程
site.name = '路条公众号';
console.log(site.name);  // => 路条公众号

注意:我们调用 getter 和 setter 的语法，它们看起来并不像一个函数调用。 Getter 和 Setter 非常重要，因为它们隐藏了内部的实现细节。

注意： 通常会在私有变量前添加下划线（_）。这里并没有真正意义上让变量私有。



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
